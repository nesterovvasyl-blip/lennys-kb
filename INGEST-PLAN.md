# Continuous Ingestion Plan

## Current approach

1. Start a session, say **"ingest continuously"**
2. Claude reads `wiki/ingested.md` and `CLAUDE.md` to find where we left off
3. Launches background agents processing 10 episodes per batch
4. Updates shared files (`wiki/ingested.md`, `wiki/index.md`, `wiki/log.md`, `CLAUDE.md`) after each batch
5. Launches next batch immediately

**Limitation**: Bound by 5-hour session usage limit. When it hits, everything stops.

**Resumption**: Start a new session, say "ingest continuously" — picks up instantly from file state.

## Remote trigger approach (not yet possible)

### What it would do
- Schedule a remote agent via `/schedule` that runs every hour in Anthropic's cloud
- Self-contained prompt reads state from files, processes next 10 episodes, updates everything
- Runs independently of any active session — survives usage limits
- Auto-disables when all 303 episodes are ingested

### Blockers
1. **Minimum cron interval is 1 hour** (not 20 min as originally wanted)
2. **lennys-kb is not a git repo** — remote agents run in Anthropic's cloud and need a GitHub repo to clone. They cannot access local files.

### Steps to unblock
1. `git init` in `lennys-kb/`
2. Create a GitHub repo (public or private)
3. Push the full project (raw transcripts + wiki)
4. Create the scheduled trigger pointing to the repo
5. Remote agent clones repo, processes batch, commits + pushes results
6. Each subsequent run pulls latest state and continues

### Trade-offs
| | Manual resume | Remote trigger |
|---|---|---|
| Setup effort | Zero | Git init + GitHub + trigger config |
| Speed | ~10 episodes/10 min | ~10 episodes/hour (min interval) |
| Automation | Requires human to start session | Fully autonomous |
| Session limit | Bound by 5-hour limit | Independent |
| Monitoring | Live in session | Check `wiki/log.md` or GitHub commits |

## Progress tracking files

- `wiki/ingested.md` — full list of ingested episodes
- `wiki/log.md` — append-only ingest log with dates and details
- `CLAUDE.md` — episode count and next batch pointer
- `wiki/index.md` — master catalog of all wiki pages
