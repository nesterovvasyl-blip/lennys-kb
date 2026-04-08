---
guest: Sri Batchu
role: Head of Growth, Ramp; formerly Head of Growth, Instacart; VP Ops, Opendoor
episode: "Lessons from scaling Ramp | Sri Batchu (Ramp, Instacart, Opendoor)"
date: 2023-06-25
topics: [growth, B2B, metrics, north-star-metric, hiring, experimentation, velocity, payback-period]
---

# Sri Batchu

> Sri Batchu is a growth leader who has built growth engines at some of the fastest-scaling companies in history — Opendoor, Instacart, and Ramp — and brings an investor/analytics mindset to what was previously a marketing or product role.

## Content

Sri was VP of Operations at Opendoor, then Head of Growth at Instacart (where he built and led a 300+ person consumer engineering team), before becoming Head of Growth at Ramp. Ramp reached $100M ARR in two years — the fastest SaaS company and the fastest FinTech company in history by that metric — and grew 4X year-over-year in a period when most companies were flat.

### Why Ramp Grew So Fast

**Product quality** is the foundation — deep PMF from a team that understood customer experience. But an overlooked early tactic: **cap table as growth strategy**. Ramp's co-founders (previously successful founders themselves) put a large number of early-stage founders and influential operators onto the cap table. Many of Ramp's earliest customers were portfolio companies of those cap-table investors, or founders directly. Word of mouth from actual users is more powerful than VC referrals; the VC opinion "matters, but not as much as another customer who's actually used the product."

The vast majority of Ramp's growth, from early days to present, comes from new customer acquisition rather than expansion within existing accounts — despite the economics of a spend management platform where customers growing means Ramp grows.

### Ramp's Growth Engine

Ramp does not have a uniquely different mix of channels vs. peers. The secret sauce: applying technology and data to every channel to make it more efficient. A dedicated **growth engineering team supports sales** with AI-driven prospecting, lead scoring, messaging prioritization, and draft response generation — a team that has existed for two years, well before AI became a buzzword. Their goal is shared with sales: pipeline generated and payback period, not product metrics. They feel ownership of the quota.

Growth team structure:
- Channel-based teams (paid marketing, lifecycle/CRM, field marketing, SEO/website)
- Product engineering team dedicated to growth + sales efficiency
- Self-serve activation engineering team
- Skunk works / innovation team for cross-channel experiments (TikTok, Reddit, referrals, first-party events)

### Velocity Culture

Ramp tracks and displays an internal counter: **days.ramp.com** — showing not just days since founding (1,529+ with decimal precision) but a constant reminder that the unit of time is a day, not a quarter. CEO Eric Glyman shows this at every board meeting and all-hands. The philosophy: never put off today what can be done today; bias to action; cycle time reduction.

In practice: fast Slack response times, immediate action item clarity even when completion is deferred, calendar auditing to ensure calendar reflects priorities. The people team provides templates for calendar audits. Building in public internally (visible work, visible wins) accelerates celebration culture — all-hands regularly achieve near-100% chat engagement.

### North Star Metrics and Translation Layers

At Instacart, the growth north star was **Monthly Active Orders (MAOs)**. But different sub-teams can't directly move MAOs — the checkout flow team moves checkout conversion. Sri's solution: a **translation layer** — a financial model updated every six months mapping each sub-team's metric to MAO impact. This allows:
- Sprint planning against local metrics
- Resource allocation and cross-team prioritization using a common currency
- Rolling up project plans to show MAO impact

The approach becomes more important as companies scale — more teams, more resources to cross-allocate. Ramp has a similar translation system, with **dollars of SQL (sales qualified lead) pipeline** as the recent north star for the growth team.

A good north star metric has two properties: (1) **clear linkage to value creation** for the business, and (2) **intuitive enough** that all teams can connect their work to it. Revenue is often too lagged; click events too leading. The sweet spot is somewhere between.

### Fail Conclusively, Not Just Fast

Most growth experiments fail (about 70% in Sri's experience). The goal is not just fail fast — it's **fail conclusively**. A non-conclusive failure is one where you ran the test but could not learn whether the hypothesis is wrong. This is especially dangerous in B2B, where sample sizes are small: the same test that Facebook validates in two hours might take two years for a B2B company.

The fix: **maximize the treatment effect**. If testing a hypothesis (e.g., "account-based marketing drives conversion"), deploy the full arsenal of tactics you believe could work, not a minimal test. If that full version doesn't work, you can confidently abandon the hypothesis. If it works, you optimize the cost later. This prevents a new executive joining and re-testing a hypothesis that wasn't actually disproved — a common failure mode.

### Payback Period over CAC

CAC is a flawed metric because it incentivizes acquiring cheap (often lower-quality) customers. LTV/CAC is better but highly assumption-laden and hard to calculate accurately for young companies. **Payback period** (how many months of contribution margin does it take to recover acquisition cost) is Sri's preferred metric because:
- It uses near-term, observable data rather than long-range projections
- It forces explicit calculation of contribution margin (not just revenue or gross margin)
- The executive team sets the acceptable payback period as a policy, and everyone optimizes to that benchmark

### B2B Channel Sequencing

A general progression Sri recommends for B2B:
1. **Founder-led sales** — early team must know how to sell
2. **First salespeople**
3. **Low-cost targeted marketing** — content, community, small events, PR
4. **Paid and brand marketing**
5. **SEO** (later, because it requires domain authority and media presence to gain traction)

The channels get more expensive and more scalable as you move down the list. SEO specifically is delayed because without backlinks and domain authority, you'll create content without traction for a long time.

### Hiring for High-Talent Density

Sri believes in designing compensation to reward 10X operators with 10X comp — not just at the executive level but across the organization. Small teams of exceptional people outperform large teams of mediocre ones. Talent density is as much about **retention and performance management** as hiring: (1) invest in high performers and accelerate their growth; (2) make hard decisions to move on people who aren't the right fit. Hesitation on the latter is how companies dilute their talent bar.

For finding great people in specific functions: use data creatively. To find great email marketers, look up which companies drive the highest % of web traffic via email (use SimilarWeb). Then source from those teams.

### Actionable Advice
- Use a "translation layer" to connect team-level metrics to the north star — update it every 6 months as you learn
- Design growth experiments to fail conclusively: maximize treatment effect to get a real answer, not a maybe
- Replace CAC with payback period as your channel efficiency metric
- Sequence B2B channels: founder-led → first salespeople → low-cost marketing → paid → SEO
- Embed engineers in sales to drive efficiency with data and automation, and give them ownership of pipeline metrics, not product metrics
- Every negotiation (especially software contracts) is possible; remember quarter-end deadlines for salespeople

### Notable Quotes
> "Culture and rituals and cadences [matter] rather than team structure. A great growth engine is one where you set very simple north star metrics — usually one, at most two — and you've created a culture of defining hypotheses that are data-driven."

> "I talk a lot about [failing conclusively] — failure is not that you didn't drive revenue, failure is not learning."

> "Payback period forces you to think about the contribution margin — how long of contribution margin from this customer does it take to payback their cost?"

> "The people that I've worked with that are highly successful — it's not the hours that someone's put in, but quality of the work and the impact."

## Sources
- [[sri-batchu]] — "Lessons from scaling Ramp | Sri Batchu (Ramp, Instacart, Opendoor)"

## See Also
- [[north-star-metric]]
- [[long-term-holdout-experiments]]
- [[velocity]]
- [[growth-model-framework]]
- [[payback-period-metric]]
- [[b2b-channel-sequencing]]
- [[talent-density]]
