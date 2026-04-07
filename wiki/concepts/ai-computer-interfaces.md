---
aliases: [ACI]
guests: [amjad-masad]
---

# AI Computer Interfaces (ACI)

> LLMs need interfaces designed for them, not repurposed human interfaces.

## Content

Amjad Masad describes AI Computer Interfaces (ACI) as the AI-native equivalent of HCI (Human-Computer Interaction). Just as decades of research optimized interfaces for human cognition, a new discipline is emerging to optimize interfaces for AI agents.

**Key insight:** LLMs are "alien creatures" trained on internet text. They are not humans, so human interfaces are suboptimal for them. Approaches like Anthropic's computer use (having AI interact with visual human interfaces) work but are expensive and slow due to image processing overhead.

**Replit's ACI design choices:**
- **Shell:** Text representation of shell state at defined increments, rather than visual terminal output
- **Editor:** Specialized tool with real-time error feedback (like a human IDE, but all text)
- **Package management:** Dedicated tool for installing packages across any language
- **Database:** Direct SQL query tools rather than visual database browsers
- **Screenshot capability:** The agent can take screenshots to verify visual output, but this is a targeted check rather than the primary interface

**The agent as a user:** Replit structured its AI agent as another user in their existing multiplayer coding system. This means the agent and human can work simultaneously on the same codebase using the same real-time collaboration infrastructure.

**Current state:** More art than science, but rapidly becoming more scientific. Key open questions include how many files to show an agent before it starts hallucinating and what the optimal editing interface looks like.

## Sources
- [[amjad-masad]] — "HCI is now ACI... turns out LLMs need interfaces that are actually quite different than humans." (Behind the product: Replit)

## See Also
- [[ai-products]]
- [[ai-non-determinism]]
