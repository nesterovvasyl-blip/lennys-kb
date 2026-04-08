---
author: bangaly-kaba
guests: [bangaly-kaba, naomi-gleit]
---
# Understand–Identify–Execute

> Facebook's growth framework — and Bangaly Kaba's shepherd — for ensuring teams invest intentional time in understanding problems before building solutions.

## Content

Popularized by [[bangaly-kaba]] who carried it from Facebook to Instagram, Instacart, Twitter (advisory), and YouTube, this framework is the antidote to the most common growth team failure mode: **identify → justify → execute** (you identify an idea, pull data to justify it, sink months building it, and the metrics are flat).

### The Core Anti-Pattern: Identify → Justify → Execute

1. Someone has an idea ("we should build X")
2. Data is pulled to justify the idea (confirmation bias baked in)
3. The team executes with conviction
4. Launch day: metrics flat
5. Post-mortem reveals the problem wasn't understood, alternatives weren't explored, users' mental models were assumed

This pattern is pervasive because execution feels productive, understand work feels slow, and teams are rarely held accountable for the quality of their understanding.

### The Correct Pattern: Understand → Identify → Execute

**Understand** is an **intentional affordance** — explicit, named work items in the roadmap with specific owners:
- Data science: pull funnel breakdowns, identify where users drop
- Engineering: instrument logging so data exists to analyze
- PM: write strategy document exploring the problem space
- UXR: run user interviews to understand mental models
- Design: prototype alternatives to test assumptions

At Instagram in 2016, Bangaly's first act was to instrument the 8-step signup funnel, which had only top/bottom logging. That understand work — figuring out where the drops were — became the foundation for all subsequent experiments.

**Identify** now happens from a foundation of real understanding — root causes, jobs to be done, the value of current alternatives.

**Execute** is then de-risked. Teams run more experiments and a higher percentage are positive.

### Recommended Allocation Ratios
- When entering a new problem space: 40–60% understand
- As the space becomes well-understood: 80–85% execute, 15–20% understand
- At Instagram with mature understand work: 15 teams × 12–20 experiments/quarter, **60–70% positive and shippable**

### What Understand Work Looks Like by Function
- **Product**: strategy docs, partnership mapping, user journey audits
- **Engineering**: code investigation, performance analysis, schema design
- **Data Science**: activation metric analysis, proxy metric research, funnel instrumentation
- **Design**: user flow walkthroughs, prototype testing
- **Go-to-Market**: pre-launch partnership discussions

### The Portfolio Approach
Every sprint should have a mix:
- Low-effort, high-confidence execution items
- Medium-effort, high-confidence execution items
- 2–3 parallel understand work streams de-risking the next sprints

The result: a "velocity multiplier" where each successive sprint is better informed, has a higher win rate, and moves faster — the opposite of what it feels like when you slow down.

## Naomi Gleit's Origin Story ([[naomi-gleit]])

Naomi Gleit was a founding member of Facebook's growth team and describes the origin of understand–identify–execute from the inside. In January 2009, the growth team stopped doing everything on the roadmap and spent the entire month on data instrumentation — logging every step of the registration flow, every step of the new user onboarding experience. Before this, the team was operating without sufficient data to make informed decisions. After this, they could see exactly where users dropped off (e.g., 20% weren't confirming their email), identify the highest-leverage interventions, and then execute with precision.

Gleit extends the principle beyond product growth: she applied the same data-driven product-driven approach to Facebook's social impact work (building peer-to-peer fundraising products) and to crowdsourced translation (community-translated the site into 100+ languages rather than hiring professional translators). In each case, the pattern was: instrument first, understand what's happening, identify the right intervention, then build.

## Sources

- [[bangaly-kaba]] — "Slow down and speed up. It's counterintuitive but if you're shipping 20 things and 15 aren't working, you'd be better shipping 10 things and having 9 of them work." (Unorthodox frameworks for growing your product, career, and impact)
- [[bangaly-kaba]] — "Understand work is an intentional affordance — you put it down as an actual item, not assume it will happen in the background." (Unorthodox frameworks)
- [[naomi-gleit]] — "Do you have the data that you need to know what you need to do on growth? If not, take the time to instrument that data." (Meta's head of product on working with Mark Zuckerberg)

## See Also

- [[bangaly-kaba]]
- [[naomi-gleit]]
- [[growth]]
- [[experimentation-culture]]
- [[marginal-user-framework]]
