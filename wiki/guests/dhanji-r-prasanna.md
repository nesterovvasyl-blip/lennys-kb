---
guest: Dhanji R. Prasanna
role: CTO, Block (formerly Square)
episode: "How Block is becoming the most AI-native enterprise in the world | Dhanji R. Prasanna"
date: 2025-10-26
topics: [ai-products, engineering-culture, org-design, ai-operations-role]
---

# Dhanji R. Prasanna

> CTO of Block (formerly Square), overseeing 3,500+ engineers; led Block's transformation into one of the most AI-native large enterprises in the world; creator of the open-source AI agent Goose.

## Content

Dhanji R. Prasanna joined Block (then Square) part-time while on parental leave, wrote an AI manifesto to Jack Dorsey arguing the company needed to take AI seriously, and was offered the CTO role as a result. Before Block, he was deeply involved in the development of Google Wave and Google Plus. Under his leadership, Block has moved from a GM structure (separate companies: Square, Cash App, Afterpay, TIDAL) to a functional organization, which Dhanji argues was the single most important step toward becoming AI-native.

Block measures AI impact as "human manual hours saved" — currently saving ~20-25% of manual work hours across all teams, with AI-forward engineering teams reporting 8-10 hours saved per week (and he emphasizes: this is the baseline, not the ceiling).

### Key Ideas

- **Functional Org Structure as AI Enabler**: Moving from GM silos (where each business unit was essentially a separate company) to a functional org (all engineers report to engineering, all designers to design) was the single biggest productivity unlock — independent of AI. It enables shared platforms, expertise transfer, and unified technical strategy. Jobs did the same when he returned to Apple.

- **Goose: Open-Source AI Agent**: Block built Goose, a general-purpose AI agent that uses MCP (Model Context Protocol, originally from Anthropic) to connect LLMs to enterprise tools — Snowflake, Salesforce, Tableau, GitHub, calendar, Slack, and essentially any system that can be wrapped in an MCP. Goose can write SQL, generate Python, build reports, manage calendar conflicts, and watch your screen to anticipate tasks. It's entirely open-source and used by many other companies. The name is a Top Gun reference.

- **Non-Technical Users as Biggest AI Beneficiaries**: The most surprising finding: non-technical teams (legal, risk, operations) get the biggest productivity gains from AI tools. An enterprise risk management team compressed weeks of work into hours by building self-service tools with Goose. This blurs the lines between functions.

- **Code Quality vs. Product Success**: "A lot of engineers think that code quality is important to building a successful product. The two have nothing to do with each other." — one of Dhanji's most counterintuitive lessons.

- **Async and Autonomous AI Work**: The next evolution is AI agents working overnight and on weekends when humans aren't there. Dhanji pushes Goose sessions from 5-7 minute median to hours. You describe multiple experiments in detail; by morning, several versions are built and you throw away the ones that don't work. New economics: throw away enormous amounts of code as normal practice.

- **Conway's Law at Scale**: "You ship your org structure." The previous GM structure meant each silo optimized independently and nobody was aligned on technical strategy. Restructuring to functional meant everyone speaks the same language, uses the same tools, and shares the same policies.

- **Use the Tool Yourself**: The main way to drive AI adoption is executive sponsorship through example. Jack Dorsey uses Goose daily. Dhanji uses Goose daily. If executives don't use the tools, the cultural change doesn't happen.

### Actionable Advice

- Before automating or buying a new tool, ask: "Do we even need this process at all?" Elon Musk's first step (do we need this?) applies before optimization.
- Identify AI opportunities by looking for processes where non-technical teams are waiting months for internal tools teams to build them something — these are high-value Goose/AI agent targets.
- Measure AI impact: track PRs, feature throughput, and self-reported hours saved, then have data scientists distill it into a single metric.
- Focus on your core DNA and purpose as a company; don't build in-house what you can buy, except for things that are core to your differentiation.

### Notable Quotes

> "Whenever I hear a stat like this, I think an important element is: this is the worst it will ever be. This is now the baseline."

> "The non-technical people using AI agents and programming tools to build things is really what's been surprising and really amazing."

> "Find your DNA and really try to optimize for what that is in a very simple and clear way."

> "A lot of engineers think that code quality is important to building a successful product. The two have nothing to do with each other."

## Sources
- [[dhanji-r-prasanna]] — "How Block is becoming the most AI-native enterprise in the world" (Lenny's Podcast, 2025-10-26)

## See Also
- [[ai-products]]
- [[ai-operations-role]]
- [[context-engineering]]
- [[ai-evals]]
