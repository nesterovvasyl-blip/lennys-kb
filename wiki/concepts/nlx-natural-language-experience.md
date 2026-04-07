---
aliases: [NLX]
guests: [aparna-chennapragada, asha-sharma]
---

# NLX — Natural Language Experience

> The design discipline for conversational and agent-based AI interfaces; NLX is to AI products what UX was to web/mobile.

## Content

Coined and championed by [[aparna-chennapragada]] at Microsoft, NLX (Natural Language Experience) is the assertion that natural-language interfaces require as much intentional design as graphical interfaces — just with different, often invisible primitives.

### Why NLX Matters
The common mistake: "With AI, the model eats the product, so there's nothing to design." This is wrong. Conversations have structure, grammar, and implicit affordances just as visual interfaces do. A podcast has different grammar than a business meeting. A customer-support chat has different conventions than an agentic research assistant. If you don't design these consciously, users get Frankenstein experiences.

### Key NLX Design Primitives

**Prompts** — no longer just a text box. The prompt is a new UI element comparable to a dropdown. How it's framed, constrained, and defaulted profoundly affects output quality and user satisfaction.

**Plans** — when an agent receives a high-level goal, it should return an editable plan. The plan is an NLX interaction pattern, not an incidental output. How editable is it? How granular? How do you show confidence?

**Showing work / progress** — how much internal reasoning should be displayed? Too verbose = running a cron job feel. Too terse = loss of confidence in whether things are going in the right direction. The right calibration depends on the task type, user sophistication, and stage of technology maturity. Personalization of this will increase.

**Follow-ups** — proactively surfacing the right next prompts. Too many = annoying. Too few = lost opportunity to guide users toward happy paths.

**Handoffs** — when does the agent ask for clarification vs. proceed? Design the grammar of when the agent pauses.

### NLX vs. GUI
GUIs are rigid but explicit. NLX is elastic but implicit. GUIs require fewer "what can I do here?" moments but constrain expression. NLX allows unbounded expression but requires users to understand the interface's grammar. Great NLX design reduces the cognitive overhead of natural language while preserving its expressiveness.

### Implications for Product Teams
- Hire or develop NLX designers as a distinct discipline
- Prototype with real natural-language interactions, not mockups
- Treat the system prompt as a product design decision as consequential as a layout
- Test the interaction grammar with users, not just the output quality

## Sources

- [[aparna-chennapragada]] — "NLX is the new UX. Conversations also have grammars, structures, UI elements — they're just invisible. What are the new principles and constructs in natural language as an interface?" (Microsoft CPO)
- [[asha-sharma]] — "GUIs → code-native interfaces. The same pattern that played out from desktop to SQL to Terraform is playing out in AI." (How 80,000 companies build with AI)

## See Also

- [[ai-products]]
- [[aparna-chennapragada]]
- [[asha-sharma]]
- [[ai-computer-interfaces]]
