---
guest: Ryan J. Salva
role: VP of Product, GitHub
episode: "The role of AI in new product development | Ryan J. Salva (VP of Product at GitHub)"
date: 2022-09-04
topics: [ai, developer-tools, product-development, incubation, big-company-innovation]
---

# Ryan J. Salva

> VP of Product at GitHub who led the incubation and launch of GitHub Copilot — one of the first AI-powered developer tools to achieve mass adoption.

## Background

Ryan J. Salva spent over a decade at Microsoft working on developer tools, including Azure DevOps and Microsoft's internal One Engineering System, before moving to GitHub. His background is unusual for a technical product leader: he studied philosophy of aesthetics and 20th-century critical theory, with a focus on how humans express creativity and communicate experience. That humanistic lens shapes everything about his approach to product.

He describes his career motivation as wanting to be "in the business of creativity" — software development as the newest human creative medium, the equivalent of what oil painting or writing were in previous centuries.

### Incubating GitHub Copilot

The origin story of Copilot is part accident, part deliberate structure. Microsoft and OpenAI had been collaborating on large language models, and the GitHub team noticed that programming languages are in some ways better subjects for LLMs than natural language — they have more constrained semantics and vocabulary.

The spark came when OpenAI was caught hammering GitHub's infrastructure to clone public repositories for training data. Rather than a confrontation, GitHub turned it into collaboration — they packaged the same Arctic Code Vault data snapshot they had already archived and gave it to OpenAI in a more structured way. From that collaboration emerged CodeX, and from CodeX emerged Copilot.

The key UX insight was inline autocomplete: instead of a side-panel suggestion that broke flow, Copilot renders suggestions in italicized gray text directly in the editor. Getting to that interaction took deliberate experimentation — including figuring out that ~200 milliseconds is the latency ceiling beyond which developers feel interrupted.

### From R&D to Product

Copilot was incubated by GitHub Next, a dedicated horizon-two/three R&D team whose job is "moonshots" — projects not expected to produce revenue in one to two years. Ryan describes the three-horizon model informally:
- Horizon 1: next year
- Horizon 2: next three years
- Horizon 3: next five years

But he emphasizes that these are better understood as measures of ambiguity and confidence than calendar dates.

The moment to graduate a project from R&D to EPD (Engineering, Product, Design) is when three things align: a representative customer with a genuine problem, medium-confidence signal that the solution works, and early prototype feedback showing "this is magical." For Copilot, that signal was the "crazy mind-blown emoji tweets" during technical preview.

The transition itself required careful people management: researchers from GitHub Next temporarily moved into the EPD squad to transfer knowledge, then gradually returned to R&D as replacement talent was hired and onboarded. The rule: don't move the researcher back until a replacement is fully in seat.

### Lessons on Big Company Incubation

Ryan's resource allocation framework for large product portfolios:
- **5–10%** of capacity on bold experimental research (horizon 2/3)
- **~25–30%** on operations — keeping in-market products meeting expectations
- **~60%** on incremental iteration of existing products

At startups, the percentages are radically different — effectively 100% on the big bet.

### AI Ethics and the Copilot Persona

Managing ethical concerns around AI-generated code required an unusual approach: anthropomorphizing the product. By framing Copilot as an "AI pair programmer," the team had a clear mental model for what constitutes appropriate behavior — it should stay focused on the task, avoid offensive or distracting output, and never try to replace the developer's judgment.

When early models produced offensive content, simple word block lists were too blunt (some medical or technical terms have legitimate uses). GitHub eventually leveraged Azure's Responsible AI models to detect sentiment in context, which was both more accurate and less brittle than the block-list approach.

### Actionable Advice
- When incubating a moonshot inside a large company, ring-fence a dedicated R&D team explicitly exempt from normal product requirements (security, accessibility, uptime, etc.)
- The graduation criteria from R&D to EPD should not be calendar-based — it must be signal-based: customer validation that the thing is "magical"
- When transitioning researchers to a product team, move them temporarily rather than permanently; staff up behind them so they can return to R&D work
- Give the new product team full ownership of roadmap — don't let R&D retain control after handoff
- Engineering fundamentals (reliability, security, privacy) feel unnatural to researchers; expect cultural change management during the transition

### Notable Quotes
> "We had a model that was amazingly good — a step level change in actual intelligence. Then marrying that against a really good use case that actually changes developers' fundamental creative process."

> "We want Copilot to augment. The idea here is really that AI is an enabler for developers to focus on the creative work, to stay in the flow, to be able to move faster."

> "I was born at the turn of the 21st century, and so I work in engineering. If I'd been born in the 1700s, I probably would've been the guy making new colors of paint and paint brushes."

## Sources
- [[ryan-j-salva]] — "The role of AI in new product development" (2022-09-04)

## See Also
- [[developer-experience]]
- [[ai-training-data]]
- [[prompt-crafting]]
