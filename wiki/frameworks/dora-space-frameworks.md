---
framework: DORA and SPACE Frameworks
created_by: Nicole Forsgren
guests: [nicole-forsgren]
topics: [developer-experience, engineering-productivity, metrics, measurement]
---

# DORA and SPACE Frameworks

> Two complementary frameworks for measuring developer productivity: DORA provides four prescriptive pipeline metrics, while SPACE offers a multi-dimensional model for holistic developer experience.

## Overview

Both frameworks were created or co-created by Nicole Forsgren. DORA emerged from her research that eventually became the book Accelerate; SPACE was developed later as a broader frame for developer experience beyond pipeline performance.

In the AI era (2025+), both frameworks need adaptation: AI has introduced feedback loops at every stage of development, changed how developers get into flow, and made code quality attribution more complex.

## Components / Steps

### DORA — Four Key Metrics
1. **Deployment Frequency** — how often code ships to production (speed metric)
2. **Lead Time for Changes** — time from code commit to code deploy (speed metric)
3. **Mean Time to Recovery (MTTR)** — how quickly you recover from incidents (stability metric)
4. **Change Failure Rate** — what percentage of deployments cause incidents (stability metric)

**Use DORA only as prescribed**: these metrics assess overall pipeline speed and stability. They don't measure developer happiness, innovation quality, or AI's contribution to individual productivity.

**AI-era limitation**: DORA was designed for feedback loops at the production end. AI introduces fast feedback much earlier in development (local build, test, and even in-flow). DORA metrics don't capture those earlier loop improvements.

### SPACE — Five Dimensions
1. **S — Satisfaction**: Developer satisfaction with tools, work, and team
2. **P — Performance**: Outcomes and results of work (not just output)
3. **A — Activity**: Counts of things done (PRs, lines of code, deploys) — useful in context, not as standalone metrics
4. **C — Communication and Collaboration**: How teams and systems communicate; proportion of work done via AI chatbot vs. human collaboration
5. **E — Efficiency and Flow**: Time to complete tasks, flow state quality, cognitive load

**AI-era addition**: Forsgren recommends adding a **Trust** dimension — developers now must evaluate whether AI-generated code is reliable, meets style standards, and is free of hallucinations before accepting it.

**SPACE's advantage**: it's a framework, not a prescriptive metric set. This makes it more adaptable to changing contexts like AI-assisted development.

## How to Apply

1. **Start with listening** before picking metrics — survey developers about their top 3 friction points and how frequently each affects them
2. **Pick metrics that map to what leadership cares about**: market share → speed; profit margin → costs; transformation → velocity
3. **Use DORA** to establish a pipeline performance baseline; track improvements to deployment frequency and lead time as DevEx work compounds
4. **Use SPACE** to choose a broader set of metrics tailored to your specific context — don't just copy-paste someone else's metric set
5. **Track code survivability rate** (how much AI-generated code persists vs. is replaced) as a new quality signal
6. **Re-evaluate metrics** as AI changes what's important — some metrics should be sunset when they no longer drive decisions

## Sources
- [[nicole-forsgren]] — "How to measure AI developer productivity in 2025 | Nicole Forsgren"

## See Also
- [[velocity]]
- [[experimentation-culture]]
- [[ai-evals]]
