---
guest: Inbal Shani
role: Chief Product Officer, GitHub
episode: "Lessons from building GitHub Copilot | Inbal Shani (GitHub CPO)"
date: 2023-12-01
topics: [github, copilot, ai-coding, developer-tools, product-led-growth, ai-adoption, developer-productivity]
---

# Inbal Shani

> Chief Product Officer of GitHub, responsible for Copilot and the developer platform — one of the most direct windows into how AI is actually changing software development at scale.

## Content

Inbal Shani joined GitHub as CPO after running product at TomTom's location technology business. She oversees GitHub Copilot, the largest AI coding assistant by adoption, and the broader GitHub platform. Her episode is notable for calibrated honesty about what AI in development is actually doing (and not doing yet), and for a significant personal failure story about change management.

### Key Ideas

- **Overhyped vs. underhyped in AI development**:
  - **Overhyped**: AI replacing human developers entirely. Copilot is a copilot, not a pilot. The analogy is intentional. The developer remains the decision-maker; AI handles the pattern-matching and boilerplate at scale. The judgment, the architecture, the "why are we building this" — those remain human.
  - **Underhyped**: AI-driven testing. Inbal argues that automated test generation is one of the most valuable but least-discussed applications of AI in development. Tests are high-effort, low-creativity work for developers. AI can generate coverage faster and more thoroughly than humans. This is already working at GitHub and most developers haven't started using it yet.

- **Copilot design philosophy — developers must WANT to use it**: The design constraint Inbal keeps returning to: Copilot cannot be something developers are told to use. It has to be something they choose. This means zero friction to the first value moment, suggestions that are good enough to make the developer faster on their first day, and a feedback model that improves without requiring explicit input. The metric is not adoption rate — it's whether developers who've used it continue using it without any prompting.

- **Developer productivity ≠ time saved; it's time-to-value**: The framing shift Inbal uses internally: the goal isn't to make developers faster in a mechanical sense. It's to reduce the time from "I have an idea" to "this is working in production." That includes code generation, but also PR reviews, documentation, onboarding new codebases, debugging sessions. The bottlenecks are rarely where companies think — they're often in context-switching, PR queue wait time, and understanding unfamiliar code, not in raw typing speed.

- **GitHub Copilot retention data — 88% of Accenture suggestions retained**: Inbal cites a stat from Accenture's Copilot deployment: 88% of Copilot's code suggestions were accepted (retained in the final code). This is not just an adoption stat — it's a quality signal. Developers are not just clicking accept; they're keeping the suggestions when they ship. This is the metric Inbal uses to counter the "it's just autocomplete" dismissal.

- **Junior developers shifting to systems thinking**: One of the most interesting structural observations — junior developers who use Copilot heavily stop spending most of their time on syntax and boilerplate and start spending more time on architecture, system design, and debugging complex interactions. This is compressing the traditional junior-to-mid-level trajectory. The worry is that juniors might skip fundamentals; the evidence so far suggests the opposite — they understand systems better because they're working at the systems level sooner.

- **GitHub Next as research-that-ships model**: Inbal describes GitHub Next — the research team that produced many Copilot prototypes — as a model worth copying. The team does genuine research, but their output is not papers: it's working prototypes that ship to production. The constraint is intentional. If your research output can't become a product, it doesn't count. This creates a very different culture than traditional R&D — researchers are invested in adoption, not just novelty.

- **Personal failure — change management at TomTom**: Inbal's most memorable story: at TomTom, she drove a significant platform transition too fast. The technology was right. The strategy was correct. The execution failed because she didn't invest enough in change management — helping the existing teams understand why, getting their input, adjusting the timeline to let the organization catch up. The lesson: the speed of a good idea is constrained by the speed at which the organization can genuinely adopt it, not just comply with it. She now explicitly builds change management planning into every major initiative.

### Actionable Advice

- If you're not using AI for test generation, start there. It's the highest ROI, lowest resistance entry point for most development teams.
- Measure developer productivity as time-to-value, not story points or commits. Map the full journey from idea to production and find the actual bottlenecks.
- For AI tool adoption: design for want-to-use, not have-to-use. The leading indicator is whether people use it on their personal projects, not whether they comply at work.
- When driving organizational change: add 30-50% more change management time than you think you need. The technical case is rarely what fails.
- Build a research function that ships to production. If the output is papers, you have a lab. If it's prototypes that become products, you have an innovation engine.

### Notable Quotes

> "Copilot is a copilot, not a pilot. That's not just branding — it's a design principle."

> "The overhyped thing is replacing developers. The underhyped thing is AI-driven testing. Everyone is sleeping on testing."

> "We don't measure adoption. We measure whether developers who've used it continue using it without anyone asking them to."

> "I moved too fast at TomTom. The technology was right. The strategy was right. I forgot that people need time to actually change, not just comply."

> "If you don't take risks, you cannot create a future."

## Sources
- [[inbal-s]] — "Lessons from building GitHub Copilot" (2023)

## See Also
- [[github-copilot]]
- [[developer-productivity]]
- [[ai-coding-tools]]
- [[change-management]]
- [[developer-tools]]
