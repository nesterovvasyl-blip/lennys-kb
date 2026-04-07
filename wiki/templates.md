# Wiki Page Templates

> Reference templates for each page type. Claude reads this when creating new pages.

## Guest Page (`wiki/guests/{guest}.md`)

Target: 400–800 words.

```markdown
---
guest: Full Name
role: Current role / most notable role
episode: "Episode title"
date: YYYY-MM-DD
topics: [topic-1, topic-2]
---

# Guest Name

> One-line bio.

## Content

1–2 paragraph bio with career context.

### Key Ideas
- **Idea Name**: 2–3 sentence explanation.

### Actionable Advice
- Concrete, implementable takeaways.

### Notable Quotes
> "Direct quote." (keep to 2–4 best quotes)

## Sources
- [[guest-name]] — "Episode title"

## See Also
- [[related-page]]
```

## Concept Page (`wiki/concepts/{concept}.md`)

Target: 200–500 words. Cross-reference all guests who discuss it.

```markdown
---
aliases: [alternate-name-1, alternate-name-2]
guests: [guest-1, guest-2]
---

# Concept Name

> One-line definition.

## Content

Definition and explanation, then each guest's perspective as a subsection or paragraph with attribution.

## Sources
- [[guest-name]] — "quote or paraphrase" (episode title)

## See Also
- [[related-page]]
```

## Framework Page (`wiki/frameworks/{framework}.md`)

Target: 200–500 words. Include steps/components.

```markdown
---
author: Guest who introduced it
guests: [guest-1, guest-2]
---

# Framework Name

> One-line summary of what it helps you do.

## Content

Origin (who created it, why). Then the framework's steps or components as a numbered or bulleted list. Practical application guidance.

## Sources
- [[guest-name]] — "quote or paraphrase" (episode title)

## See Also
- [[related-page]]
```

## Topic Page (`wiki/topics/{topic}.md`)

Target: 500–1500 words. Synthesis across guests — this is the most valuable page type.

```markdown
---
guests: [guest-1, guest-2, guest-3]
related_raw_index: topic-name.md
---

# Topic

> One-line framing.

## Content

Synthesize perspectives from all guests who discuss this topic. Organize by theme or subtopic, not by guest. Each paragraph should weave together multiple viewpoints. Attribute with [[wikilinks]].

## Sources
- [[guest-name]] — "quote or paraphrase" (episode title)
(list all contributing guests)

## See Also
- [[related-page]]
```

## Comparison Page (`wiki/topics/{topic-a}-vs-{topic-b}.md`)

Target: 300–800 words. Created via Query closure or user request.

```markdown
---
guests: [guest-1, guest-2]
type: comparison
---

# Topic A vs. Topic B

> One-line framing of the comparison.

## Content

What they share, where they diverge, when to use each. Use a table if the comparison has 3+ dimensions:

| Dimension | Topic A | Topic B |
|-----------|---------|---------|
| ...       | ...     | ...     |

Prose synthesis below the table.

## Sources
- [[guest-name]] — "quote or paraphrase" (episode title)

## See Also
- [[related-page]]
```
