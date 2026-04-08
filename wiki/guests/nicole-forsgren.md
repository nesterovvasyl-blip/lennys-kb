---
guest: Nicole Forsgren
role: Senior Director of Developer Intelligence and Core Developer, Google (formerly VP Research & Strategy, GitHub)
episode: "How to measure AI developer productivity in 2025 | Nicole Forsgren"
date: 2025-10-19
topics: [developer-experience, engineering-productivity, devex, ai-tools, metrics, measurement]
---

# Nicole Forsgren

> Creator of the DORA and SPACE frameworks for measuring developer productivity, author of Accelerate, and the leading authority on developer experience in the age of AI.

## Content

Nicole Forsgren created the most widely used frameworks for measuring developer productivity: DORA (four key metrics assessing pipeline speed and stability) and SPACE (a multi-dimensional framework for developer experience). She co-wrote Accelerate, the foundational book on high-performing technology organizations. She was previously VP of Research and Strategy at GitHub and is now Senior Director of Developer Intelligence and Core Developer at Google. She is co-authoring a new book, Frictionless, with Abi Noda (co-founder of DX, which sold to Atlassian for $1B).

This episode is a follow-up to her first appearance (recorded ~2.5 years earlier). The prior conversation barely touched AI; this one focuses almost entirely on how AI is reshaping the measurement and improvement of developer experience.

### Why Traditional Productivity Metrics Fail in the AI Era

Most productivity metrics are easy to game. Lines of code — always a poor metric — becomes absurd with AI, since you can prompt an LLM to write the longest, most verbose code imaginable. But more subtly, even good frameworks like DORA need to be adapted:

- **DORA** was designed to measure pipeline speed (deployment frequency, lead time) and stability (MTTR, change fail rate). These metrics are still valid for their prescribed purpose. But AI has introduced feedback loops at every stage of development — not just at the production end — that DORA wasn't designed to capture.
- **SPACE** (Satisfaction, Performance, Activity, Communication/collaboration, Efficiency/flow) holds up better because it's a framework, not a prescriptive set of metrics. It lets you pick what to measure. Forsgren suggests adding a "Trust" dimension for the AI era: developers must now evaluate whether AI-generated code is reliable, meets style standards, and avoids hallucinations.

Code survivability rate (how much AI-generated code persists vs. is replaced) is a promising new metric that can also reveal downstream quality effects and fine-tuning loop risks.

### How AI Is Changing Flow State and Cognitive Load

Three pillars of developer experience: **flow state**, **cognitive load**, and **feedback loops**.

AI both disrupts and potentially enhances flow state:
- It interrupts traditional deep work by fragmenting attention into prompt→review→integrate cycles
- But senior engineers who master agentic workflows have found a new kind of flow — directing parallel agents across system components, staying at a high-level architectural perspective while agents execute in parallel

Key insight: AI may enable productive 45-minute work blocks, not just 2-hour deep dives, because the machine helps you re-enter context quickly. The "getting into flow" overhead shrinks if the AI can recap where you left off and generate system diagrams.

Forsgren expects the entire nature of developer work to shift toward orchestration and review, more like an engineering manager coordinating junior developers.

### The Frictionless 7-Step Framework

From her forthcoming book (co-authored with Abi Noda):
1. **Start the journey** — listening tour, synthesize what you learn, visualize current workflow and tools
2. **Get a quick win** — small, visible improvement; share it widely to build momentum
3. **Use data to optimize** — establish data foundation; surveys for fast signal; collect new instrumentation
4. **Decide strategy and priority** — of all the things that are broken, what do you fix next? Evaluation frameworks for prioritization
5. **Sell your strategy** — get feedback, communicate why this is the right direction now
6. **Drive change at your scale** — grassroots (local scope) or top-down (global scope) change management approaches
7. **Evaluate progress and show value** — then loop back

DevEx initiatives follow a J-curve: quick wins up front, then a dip while you build infrastructure and telemetry, then compounding benefits. Knowing this prevents teams from abandoning the effort in the dip.

### What to Measure First

For companies just starting: don't start with instrumentation — start with surveys.
- Ask developers: "What were the top 3 things that slowed you down or frustrated you this week?" (force them to pick only 3; unlimited lists create noise)
- Ask follow-up: how often does each affect you? (daily, weekly, quarterly)
- This surfaces both the nature of the friction and its intensity, giving a weighted score

Avoid happiness surveys — too many external factors contaminate the signal. Satisfaction surveys (specifically about tools and workflows) are more actionable.

For measuring AI impact, link to what leadership cares about:
- **Market share focus** → measure speed: feature to customer, feature to experiment
- **Profit margin focus** → measure cost savings: cloud costs, vendor spend reduction, recovered developer time
- **Transformation focus** → frame everything as enabling change

### Signs Your Engineering Team Could Move Faster

- Builds are always breaking or flaky tests are constant
- High switching costs between codebases or orgs (people avoid changing teams because setup takes as long as onboarding)
- Long provisioning or environment setup times
- People "living with" a known process problem rather than fixing it (e.g., printing something and walking it down four flights of stairs)

The first improvement is almost always a process change, not a technical one. The most impactful early wins often require no engineering: just changing who signs off on what, or how information flows.

### DevEx as a Product

Forsgren's key recommendation: apply PM thinking to DevEx work.
- Define the problem and users
- Create MVPs and run experiments; get fast feedback
- Know your "addressable market" (which teams, which workflows)
- Have a comms plan and a go-to-market — internal products fail without adoption
- Track metrics as a product, not just as overhead
- Plan sunsetting: are old metrics still driving good decisions?

### Actionable Advice
- Start DevEx work by talking to developers, not by building tools
- Use surveys with forced prioritization (top 3 problems) before building instrumentation
- Apply PM product lifecycle thinking to DevEx initiatives
- Measure what leadership cares about — translate the same improvement into their language
- Don't use happiness surveys; use satisfaction surveys tied to specific tools and workflows
- Expect a J-curve: quick wins, then dip, then compounding returns
- Better documentation and comments improve AI tool output — invest in them

### Notable Quotes
> "Most productivity metrics are a lie. If the goal is more lines of code, I can prompt something to write the longest piece of code ever. It's just too easy to game that system."

> "Most teams can move faster. But faster for what? We can ship trash faster every single day. We need strategy and really smart decisions to know what to ship."

> "If DevEx is poor, everything else just isn't going to help. The best processes, the best tools... if the DevEx is bad, everything kind of takes."

> "Go talk to people and listen. Start with listening and not with tools and automation."

## Sources
- [[nicole-forsgren]] — "How to measure AI developer productivity in 2025 | Nicole Forsgren"

## See Also
- [[velocity]]
- [[experimentation-culture]]
- [[ai-evals]]
- [[product-ops]]
