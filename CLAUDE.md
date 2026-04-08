# Lenny's Podcast — LLM Knowledge Base

This is an LLM-maintained knowledge base built from 303 Lenny's Podcast episode transcripts, following Andrej Karpathy's "LLM Knowledge Bases" pattern.

## Core Principle

**Knowledge compounds.** Every ingest, every query, every exploration adds to the wiki. The LLM is a compiler, not a retriever — it pre-processes raw sources into an interconnected wiki so queries reference synthesized knowledge rather than re-deriving answers each time. The human curates sources and steers direction; the LLM handles summarization, cross-referencing, filing, and consistency.

## Architecture

```
lennys-kb/
├── CLAUDE.md              # This file — schema and workflow instructions
├── raw/                   # Source transcripts (NEVER modify)
│   ├── episodes/{guest}/transcript.md
│   └── index/{topic}.md   # 89 topic→episode mappings (use for topic page seeding)
└── wiki/                  # LLM-generated wiki (Claude maintains this)
    ├── index.md           # Master catalog — one-line summaries, used for query routing
    ├── ingested.md        # Full list of ingested episodes
    ├── log.md             # Append-only ingest log
    ├── guests/            # One page per guest — bio, key ideas, quotes
    ├── concepts/          # Concept/term pages (e.g., product-market-fit.md)
    ├── frameworks/        # Named frameworks guests describe (e.g., racecar-framework.md)
    └── topics/            # Topic synthesis pages (e.g., growth.md, pricing.md)
```

## Rules

1. **NEVER modify anything in `raw/`** — it is immutable source material.
2. All wiki output goes in `wiki/`.
3. Use `[[wikilinks]]` for cross-references between wiki pages.
4. Keep pages focused — one concept/framework/guest per page.
5. Always update `wiki/index.md` and `wiki/log.md` after each ingest batch.
6. **Shared file writes**: When running concurrent agents, only write to `wiki/index.md`, `wiki/log.md`, and `wiki/ingested.md` from the main conversation — never from agents. Agents write only to their own guest/concept/framework/topic pages.
7. **Index-first retrieval**: For queries, always read `wiki/index.md` first to locate relevant pages. The index is the routing layer — avoid scanning directories.
8. **Closure**: Every valuable exploration gets filed back into the wiki. A good answer to a user question becomes a wiki page. This is how knowledge compounds.

## Page Types & Templates

Templates are inlined in agent prompts (see Technical Notes). No need for agents to read `wiki/templates.md`.

| Type | Directory | Target length | Purpose |
|------|-----------|---------------|---------|
| Guest | `wiki/guests/` | 400–800 words | Bio, key ideas, quotes from one episode |
| Concept | `wiki/concepts/` | 200–500 words | One idea, multiple guest perspectives |
| Framework | `wiki/frameworks/` | 200–500 words | Named method with steps/components |
| Topic | `wiki/topics/` | 500–1500 words | Cross-guest synthesis (most valuable) |
| Comparison | `wiki/topics/` | 300–800 words | Side-by-side analysis with tables |

**Naming**: All filenames use `kebab-case.md`. Guest pages match the `raw/episodes/` directory name. Concepts/frameworks use the shortest unambiguous name.

## Workflows

### Ingest (batch mode)

Process a batch of episodes. For each episode:

1. Read `raw/episodes/{guest}/transcript.md` — start with the YAML frontmatter to get guest name, episode title, and description before reading the full transcript
2. Extract: guest bio, key ideas, memorable quotes, frameworks, actionable advice
3. Create `wiki/guests/{guest}.md`
4. For each significant concept or framework mentioned:
   - **Glob** `wiki/concepts/` or `wiki/frameworks/` to check if the page exists before creating
   - If the page exists, **merge** — read the existing page first, then add the new guest's perspective. Update frontmatter `guests` list and Sources. Do not rewrite existing content.
   - If the page doesn't exist, create it
5. **Do NOT update existing topic pages** (`wiki/topics/*.md`). Instead, include topic tags in the agent's return summary. Topic pages are updated in dedicated synthesis passes.
   - Exception: agents MAY create a **new** topic page if no page exists for a clearly significant topic.
6. Return a structured summary of created/updated pages to the main conversation, including a `topic_tags` list mapping each guest to relevant topics.

**After the agent returns**, the main conversation updates shared files:
- `wiki/index.md` — add new page entries
- `wiki/log.md` — append ingest log entry
- `wiki/ingested.md` — add episode to the list
- `CLAUDE.md` — update the episode count and next-batch pointer
- **Git commit, push, create PR, and merge** after each batch completes and shared files are updated

**Multi-guest episodes**: Create one guest page per person. Shared ideas go on concept/framework pages with both guests cited.

**Duplicate episodes**: Some guests appear multiple times in `raw/` (e.g., `april-dunford` and `april-dunford-20`). Check `wiki/ingested.md` skipped list. If a duplicate, skip it. If genuinely different, merge new ideas into existing guest page.

**Non-guest episodes to skip**: `teaser_2021`, `interview-q-compilation`, `eoy-review` — compilations/promos. Add to skipped list in `wiki/ingested.md`.

**Transcript chunking**: Read frontmatter first (first 20 lines). Then check line count — read short transcripts (<500 lines) in one pass, longer ones in ~500-line chunks.

**Batch size**: 20 episodes per batch, split across **2 parallel agents of 10** each. Each agent handles a non-overlapping set of episodes to avoid concept page conflicts.

### Topic Synthesis Pass

**Run after every 5 batches** (batches 10, 15, 20...). Dedicated agent reads all guest pages created since last synthesis, then updates topic pages with new perspectives.

Last topic synthesis: **Batch 7** (topics current through episode 67)
Next topic synthesis due: **Batch 12**

### Ingest (interactive mode)

For exploring a single episode in depth with the user:

1. User says **"ingest {guest-name}"** or **"explore {guest-name}"**
2. Read the transcript, discuss key takeaways with the user
3. User can steer: "dig into the framework they describe", "what's the actionable advice?", "how does this relate to [[growth]]?"
4. Write wiki pages based on the conversation
5. Update shared files

This mode prioritizes depth and user involvement over throughput.

### Query

1. User asks a question about the knowledge base
2. Read `wiki/index.md` to locate relevant pages, then read those pages
3. If wiki pages are insufficient, search raw transcripts for additional context
4. Synthesize answer with citations to specific episodes/guests
5. **Closure rule**: If the answer is substantial, reusable, or connects ideas across 3+ guests — save it as a new wiki page (concept, topic, or comparison). Log it. This is how the wiki compounds.
6. **Output formats**: Answers can be prose, comparison tables, or bulleted lists — match the format to the question. Comparison questions → table format → save as a comparison page.

### Compare

User says **"compare X and Y"** (guests, concepts, or frameworks).

1. Read the relevant wiki pages for both sides
2. Build a comparison table (dimensions × perspectives)
3. Add prose synthesis below the table
4. Save as `wiki/topics/{x}-vs-{y}.md` using the comparison template
5. Update `wiki/index.md` and `wiki/log.md`

### Lint

Periodic health check. Run with **"lint wiki"**.

**Structural checks:**
1. Find orphan pages (not linked from index or other pages)
2. Find concepts referenced in `[[wikilinks]]` but without their own page
3. Check for duplicate/overlapping pages
4. Verify all pages have YAML frontmatter
5. Verify `wiki/index.md` is complete (no pages missing from catalog)

**Content checks:**
6. Find contradictions between pages (e.g., two pages attributing the same framework to different guests)
7. Find superseded claims — newer episodes may update or contradict earlier ones
8. Identify topics with few cross-references (signals missing synthesis)
9. Flag guest pages that are thin (<200 words) relative to transcript length

**Report and fix** — output a summary, then fix structural issues automatically. Flag content issues for user review.

## Ingest Progress

**234 / 303 episodes ingested** (last updated: 2026-04-07)

Full list: `wiki/ingested.md`

Next batch starts at: **shishir-mehrotra** (alphabetically after shaun-clowes)

## Commands

| Command | What it does |
|---------|--------------|
| **"ingest next batch"** | Process next 10 episodes (batch mode) |
| **"ingest continuously"** | Run batches back-to-back via background agents |
| **"ingest {guest}"** / **"explore {guest}"** | Interactive single-episode deep dive |
| **"compare X and Y"** | Side-by-side analysis → comparison page |
| **"lint wiki"** | Structural + content health check |

## Technical Notes for Claude

- Use `Agent` tool with `run_in_background: true` and `model: sonnet` — **launch 2 agents in parallel** per batch (10 episodes each, 20 total per batch)
- **Inline templates in agent prompt** — do NOT have agents read `wiki/templates.md` (saves a tool call per agent)
- **Do NOT pass a list of existing pages in the agent prompt** — instead, tell agents to `Glob` the relevant directory before creating a page to check if it exists
- Agents write guest/concept/framework pages directly. **Agents do NOT update existing topic pages** — they return topic tags for the synthesis pass
- Agent does NOT write to `index.md`, `log.md`, or `ingested.md` — main conversation handles these
- After both agents complete and shared files are updated, launch the next batch immediately
- Do NOT bring transcript content into the main conversation — keep it in agents
- **Merge rule**: When updating an existing concept/framework page, read it first, add the new guest's perspective, update frontmatter and Sources. Never overwrite existing content.
- **Error recovery**: If an agent fails mid-batch, check which guest pages were written (`wiki/guests/`). Re-run only the unprocessed episodes.
