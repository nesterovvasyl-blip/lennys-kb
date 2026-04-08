---
guest: Shweta Shrivastava
role: Senior Director of Product Management, Waymo; formerly CPO at Nauto, Head of PM at Amazon Web Services
episode: "Product lessons from Waymo | Shweta Shrivastava (Waymo, Amazon, Cisco)"
date: 2023-04-09
topics: [product-management, autonomous-vehicles, hardware-software, metrics, hiring, career, mvp]
---

# Shweta Shrivastava

> Shweta Shrivastava is a senior product leader at Waymo who has built product teams across hardware-software systems, cloud infrastructure, and consumer-facing technology — and whose lessons about working backwards, knowing what you're not building, and disrupting yourself apply far beyond self-driving cars.

## Content

Shweta joined Waymo after serving as CPO at Nauto (AI-focused driver automation safety) and heading product management for AWS database and analytics services. She previously worked at Cisco. At Waymo, her team owns three areas: the onboard software governing vehicle behavior and trajectory, simulation tools for validation, and the commercial ride-hailing business scaling.

### Building Product at Waymo vs. Traditional Software

The most significant differences: PMs must go technically deep (understanding ML model behavior, validation pipelines, sensor systems), must be comfortable with very long time horizons (the "long game"), and must be genuinely driven by the mission of eliminating road deaths — about 1.35 million annually, mostly attributable to human driving error. The MVP bar is radically higher: you cannot ship a "minimum viable" self-driving car that is unsafe. Safety is non-negotiable as a baseline before iteration can begin.

The car's body language — how it negotiates merges, how it handles downhill slopes, how it handles pedestrians with non-standard intent — is designed through deep learning on human driving data, filtered to discard bad driving patterns. The system learns social norms by region (SF pedestrians may cross against signs; elsewhere they may not). The experience is designed to feel "credible, predictable, and trustworthy" — not robotic. In practice: riders who are initially amazed report that within five minutes, riding in a Waymo feels completely natural. That naturalness is not accidental.

One notable design insight: a Waymo adheres to the speed limit by default, but designers found that vehicles should slow down approaching downhill grades — even when staying within the limit — because human drivers do, and riders found it more natural and trustworthy. Explicit design of naturalistic behavior, not just rule-following, builds rider trust.

### Metrics at Waymo

Two broad categories: (1) **Commercial/Operational Metrics** — trips per week, daily/weekly active users, funnel metrics, cost per ride; (2) **Driver Performance Metrics** — safety (collisions per 100K miles vs. human benchmark), compliance with road rules, "adequate progress" (stops and strands, ability to navigate dense traffic), and road impact (did the vehicle impede other traffic?). The safety goal is simple to state: drive safer than humans, measured against a human driving benchmark.

### Keeping Stakeholders Bought In on Long-Term Investments

Key insight: show meaningful progress — not just technology milestones but commercial deployments. The "rubber meets the road" phase converts technology ambition into business credibility. Don't manufacture optics; focus on creating genuine value for users. Investors will see through artificial brownie points. At Waymo's scale, continued investment comes from accelerating their own milestones beyond their own projections.

### Core PM Lessons

**Work backwards from the customer problem**: Shweta learned this at Amazon through the PR/FAQ process — PMs write the press release for a finished product before they start building. Forces the team to articulate value proposition, not technology or implementation. She adapted this at Waymo: different teams have their own versions of "working backwards," but the core practice of starting with the user problem is universal.

**Know what you're not building**: In large companies and startups alike, saying no is as important as saying yes. Products trying to be all things to all people go nowhere. The classic innovator's dilemma: large market leaders become incremental and get disrupted. Product leaders must push companies to disrupt themselves. At Amazon, Shweta drove Honeycode (a no-code application platform) — new territory for Amazon, which was infrastructure-focused. Companies that challenge themselves before competitors do survive.

**The underrated PM skill is listening and empathy**: The sexy skills (influencing without authority, writing PRDs, prioritizing) are visible. Listening with an open mind and challenging your own assumptions are more foundational but less taught. The tell: if there's never conflict or contention, you might not really be listening. Genuine listening means actively probing against your own assumptions, not just gathering input.

**On getting promoted**: Focus on impact, not promotion. Optimize for the right things for the business, make your ambitions known to your manager, and then work on genuinely impactful projects. Managers can tell when someone is maneuvering for a title — and it's a negative signal.

### Actionable Advice
- Write a PR/FAQ for your product before you build it — the discipline of writing about the finished product first clarifies the value proposition
- Know explicitly what you are NOT building; a product that tries to be all things to all people usually doesn't go anywhere
- Disrupt yourself before someone else does — if you're leading in a market, proactively ask what would threaten your position and build toward that
- If a long email thread has gone past seven exchanges without resolution, get on a call (the "rule of seven")
- Focus on real impact, not optics, to build stakeholder buy-in for long-term investments

### Notable Quotes
> "Are you proactively trying to challenge your own assumptions? If there's no conflict, if there's no contention, then something is missing."

> "It's also very important to know what you're not building. A product that tries to be all things to all people usually doesn't end up going anywhere."

> "You have to disrupt yourself before somebody else does, because it's inevitable."

> "Focus on the impact. If you try to maneuver too much for a promotion, it becomes visible and it's not a positive signal to the organization."

## Sources
- [[shweta-shriva]] — "Product lessons from Waymo | Shweta Shrivastava (Waymo, Amazon, Cisco)"

## See Also
- [[working-backwards]]
- [[minimum-lovable-product]]
- [[product-market-fit]]
- [[crossing-the-chasm]]
