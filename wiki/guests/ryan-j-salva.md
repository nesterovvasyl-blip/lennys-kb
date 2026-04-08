---
guest: Ryan J. Salva
role: VP of Product at GitHub (Microsoft)
episode: "The role of AI in new product development | Ryan J. Salva (VP of Product at GitHub)"
date: 2022-09-04
topics: [ai-products, incubation, product-development, github-copilot, r-and-d, developer-tools]
---

# Ryan J. Salva

> VP of Product at GitHub who incubated and launched GitHub Copilot, Ryan Salva is a practitioner at the intersection of AI, developer tools, and large-company product innovation.

## Bio

Ryan J. Salva spent over 10 years at Microsoft before joining GitHub, where he leads product for multiple product lines including GitHub Copilot, Codespaces, and developer security tools. His academic background is in philosophy of aesthetics and 20th-century critical theory — an unusual foundation for a developer-tools leader, but one he credits with giving him an appreciation for human communication, dialogue, and how new mediums reshape creativity. He draws a direct line from philosophy to product work: "I wanted to be in the business of creativity."

## Key Ideas

### Incubating Big Bets Inside Large Companies

Copilot originated in GitHub's R&D group "GitHub Next," whose mandate is to explore second- and third-horizon projects — things that might be relevant three to five years out, measured more by ambiguity and confidence level than calendar dates. Ryan's three-horizon rough allocation:
- **5–10%** of team capacity: truly uncertain experimental bets (GitHub Next work)
- **25–30%**: operational maintenance of in-market products
- **60%+**: incremental improvements to existing products

The transition from GitHub Next to a shipping product followed a specific pattern:
1. Researchers at Next generate a promising prototype
2. Signal emerges from customers: "This is magical, this does something I couldn't do on my own"
3. A small number of researchers transfer to a new EPD (Engineering, Product, Design) squad for a **finite period**, seeding the product team while doing knowledge transfer
4. The EPD team takes over; researchers return to GitHub Next
5. New EPD squads hire around the researchers' seed to carry the product forward

The critical insight: **researcher transfers must be based on replacement in seat, not calendar dates.** You can't pull the researcher back until someone has actually absorbed the domain expertise. Forcing a handoff by deadline creates capability gaps.

### The Copilot Origin Story

Copilot's origin was almost accidental. OpenAI was scraping GitHub's public repositories (a massive clone operation that triggered GitHub's infrastructure team). Rather than fight it, GitHub packaged the data responsibly through the Arctic Code Vault snapshot and brought it to OpenAI. The question became: what can we do with large language models trained on public code?

Key discovery: code languages are much more constrained semantically than natural languages — fewer "words," stricter grammar. This makes code particularly well-suited for language model training. The team then spent months experimenting with **prompt crafting** (how to structure the input to the model to get useful suggestions) and UX (the gray italicized inline autocomplete was the result of many experiments, not an obvious choice). Latency experiments determined ~200ms as the sweet spot — fast enough to stay in developer flow.

### AI as Augmentation, Not Replacement

Ryan is explicit: Copilot's goal is not to replace developers. The "AI pair programmer" framing is deliberate — a pair programmer whispers suggestions but doesn't write code unilaterally. This framing also governs content moderation: you wouldn't tolerate a pair programmer who injects offensive or irrelevant content while you're trying to work. The goal is to remove drudgery (syntax recall, parameter ordering, boilerplate data structures) so developers can focus on creative, outcome-oriented work.

His vision for 5–10 years: AI infuses the entire dev stack — PR summarization, code review, build queue management, security scanning — progressively removing "rote memorization of syntax" so engineers focus on design patterns and outcomes.

### Scaling Ethical AI Products

Copilot faces challenges that most products don't:
- **Supply chain for compute**: specialized GPUs in scarce global supply
- **Community trust**: training on public code requires ongoing dialogue about consent, attribution, and responsible AI
- **Content moderation**: block lists are fragile; they eventually transitioned to Azure's Responsible AI models for semantic-level content detection
- **Skepticism as healthy**: Ryan genuinely wants developers to be skeptical of Copilot, treating it as a spur to keep improving safety and quality rather than a problem to be suppressed

### Hiring Interview Technique: Teach Me Something in One Minute

For early-to-mid career PMs, Ryan asks candidates to teach him something new in one minute, evaluated on three criteria: **completeness** (did they finish?), **complexity** (was the topic substantive?), and **clarity** (did he actually learn something?). He notes the most impressive answer was from a university student who taught him about 18th century art's connection to religious trends of the period.

## Key Quotes

> "What I care about is helping people create... software development and the worlds it creates wasn't possible maybe 50, 60 years ago." — Ryan J. Salva

> "We do not want Copilot auto generating code where a thinking, reasoning, breathing human being is not on the other side of that keyboard." — Ryan J. Salva

> "The criteria for moving researchers back into their R&D team can't be based on a calendar. It needs to be based on replacement in seat." — Ryan J. Salva

> "We want AI to augment. The idea is that AI is an enabler for developers to focus on the creative work, to stay in the flow." — Ryan J. Salva

## Actionable Advice

- Ring-fence a small team (5–10% of capacity) for genuinely uncertain exploratory bets, fully separated from operational product teams
- When transitioning research projects to product, bring a subset of researchers into the EPD squad temporarily — don't just "hand off" the knowledge
- Only transition researchers back when domain knowledge has fully transferred — never on a calendar deadline
- Give the product team full ownership of the roadmap; don't outsource innovation exclusively to R&D
- Teach engineers about engineering fundamentals through cultural change management, not mandates
- Frame AI products around a strong "use case persona" — the framing helps guide ethical and content decisions
- Expect healthy skepticism from your user community; welcome it as a forcing function for quality

## Related Pages

- [[concepts/developer-experience]]
- [[concepts/ai-training-data]]
- [[concepts/ai-evals]]
- [[topics/ai-products]]
- [[topics/incubation-and-r-and-d]]
