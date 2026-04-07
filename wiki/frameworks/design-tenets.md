---
author: Bob Baxley
guests: [bob-baxley]
---

# Design Tenets

> Opinionated decision rules that resolve recurring design debates once and for all — more useful than principles because they're specific enough to disagree with.

## Content

Design tenets, as defined by [[bob-baxley]], are distinct from design principles. Standard design principles ("simple," "clear," "beautiful," "fast") are platitudes — no one argues the opposite, so they don't help you make decisions. Tenets are decision-making tools: explicit, opinionated answers to the recurring debates a team keeps having.

The concept came from Baxley's experience at ThoughtSpot, where he realized he couldn't have command-and-control over a product with hundreds of engineers spread across India and the US. He needed to move from control to choreography — to set shared rules that would allow the right decisions to be made independently, at any level.

**How to find your tenets**: Pay attention to debates that keep recurring in your team — places where people consistently split into two camps and no one can resolve it without escalating. Those are your candidates. Have the debate once, make an opinionated decision, and encode it.

**Properties of good tenets**:
- You can state the opposing position (otherwise it's not a real tenet, it's a platitude)
- They apply at the *design strategy* level, not the feature level
- They must be memorizable — 3–4 max
- They should be context-specific to your product and moment

**ThoughtSpot examples**:
1. *Documentation is a failure state* — If users need to read a manual, the product failed them. Work backward from self-evident interfaces.
2. *Start simple, let users opt into complexity* — Default to the approachable experience; power users unlock the full feature set, not the reverse.
3. *The whole product should look and feel like it came from a single mind* — Combats the natural tendency of distributed teams to optimize their feature in isolation.

**Keynote example (from Steve Jobs)**: When starting Keynote, Jobs gave the team three tenets: (1) It should be difficult to make ugly presentations; (2) Focus on cinematic quality transitions; (3) Optimize for innovation over PowerPoint compatibility. That third tenet in particular eliminated years of potential debate — the team knew which way to go without escalating.

Baxley distinguishes tenets from opinionated software (see [[opinionated-defaults]]): tenets are internal decision rules for the design team; opinionated software is the externally expressed opinion encoded in product constraints.

## Sources
- [[bob-baxley]] — "Tenets are really decision-making tools... you have to be opinionated, but that's how you're going to win. There's no unopinionated software that's been successful." (35 years of product design wisdom)

## See Also
- [[bob-baxley]]
- [[opinionated-defaults]]
- [[taste-as-competitive-advantage]]
