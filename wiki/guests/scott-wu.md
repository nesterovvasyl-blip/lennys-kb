---
guest: Scott Wu
role: Co-founder and CEO, Cognition (makers of Devin)
episode: "Inside Devin: The AI engineer that's set to write 50% of its company's code this year"
date: 2025-05-04
topics: [ai-engineering, autonomous-agents, future-of-software-engineering, jevons-paradox, hiring, startup-execution]
---

# Scott Wu

> Co-founder and CEO of Cognition, building Devin — the world's first autonomous AI software engineer.

## Background

Scott Wu is a competitive programming veteran who previously ran Lunchclub (an AI-powered professional networking product for five years) before co-founding Cognition with Steven and Walden in late 2023. He and his co-founders met through competitive programming and math competitions and maintained close relationships across a decade of separate AI careers before coming together. Cognition launched Devin in March 2024 and released Devin 2.0 in early 2025. The company operates with a team of roughly 26-27 people, 15 of whom are engineers — and each engineer works with up to five concurrent Devins.

### What Devin Is

Devin is a fully autonomous AI software engineer. Unlike coding assistants (which suggest code inline), Devin operates asynchronously through integrations with Slack, GitHub, and Linear. You tag Devin on an issue, Devin plans and executes, makes pull requests, debugs CI failures, and iterates based on feedback. It maintains a persistent knowledge representation ("Devin Wiki") of your codebase architecture that improves over time.

Devin is best on well-defined tasks with clear feedback loops — bug fixes, front-end feature requests, adding documentation and tests. The right framing is: give Devin **tasks, not problems**. The harder the scoping and verification problem, the more human oversight is needed.

At Cognition itself, approximately 25% of all pull requests are authored by Devin (as of mid-2025), with a target of over 50% by end of year. Engineers typically work with 4-5 concurrent Devins.

### From Bricklayer to Architect

Wu's central thesis about how AI transforms software engineering: programming has always been about telling computers what you want, and that remains true whether you're writing assembly, Python, or instructing a Devin. The soul of software engineering — defining the problem, thinking through architecture, mapping the solution — represents about 10% of the average engineer's time. The other 90% is implementation drudgery (Kubernetes errors, migrations, version bumps, bug reports).

Devin enables engineers to shift from bricklayer (doing the implementation) to architect (specifying what should be built). This is not about replacing engineers — it is about enabling them to do the part of engineering that actually requires human judgment at a dramatically higher rate. Wu expects total demand for engineers to *increase* as building becomes cheaper (citing Jevons' Paradox).

### The Eight Pivots

Cognition went through roughly eight pivots within coding agents before landing on Devin's current form. Early work focused on competitive programming agents (agentic loops for contest problems). The key bets from the start were: (1) reinforcement learning was the next paradigm shift in capabilities — moving from imitation learning (reading internet text) to high-compute RL (learning from automated code execution feedback), and (2) the product experience would shift from text-completion (like GitHub Copilot) to fully autonomous agentic systems.

Features added over time through iteration: Slack integration, GitHub/Linear integrations, interactive planning phases, the ability to touch up Devin's code mid-session, Devin Wiki for codebase representation, and confidence-level reporting. The product metaphor evolved from "hand it a task and it runs" to treating Devin genuinely like a junior engineer you work alongside.

### Moats Are Stickiness

On competitive defensibility, Wu makes an important distinction: **moats** (barriers that prevent entry) are rare in AI. What matters is **stickiness** — the degree to which a product becomes more valuable the longer you use it. For Devin, stickiness comes from: (1) Devin's growing knowledge of your specific codebase and workflows, (2) multiplayer effects (Devin accumulates knowledge from the whole team, not just one user), and (3) the difficulty of switching once your development workflows are deeply integrated.

### AI Is Not Hardware-Constrained

Wu argues that previous technology waves (PC, internet, mobile) all had hardware distribution bottlenecks that slowed adoption to a "steady year-over-year" curve. AI has no such hardware constraint. Once AI tools cross the inflection point of practical usefulness, adoption can be explosive. He believes we've already passed that inflection point in AI coding.

### Startup Execution as Clichés Taken Literally

Wu's counterintuitive startup insight: the clichés (hire great people, move fast, build what people want, stay close to customers, think about where things are going) are not things to know — they are things to take more literally than you imagine. Cognition went from hackathon to company to launch to first customers in five months. For hiring, Wu flew to North Carolina to have dinner with a candidate's parents to negotiate a part-time school arrangement so the candidate could join full-time. The stories of doing these ordinary things to an extraordinary degree are what make the difference.

### Actionable Advice
- Give Devin tasks, not problems — scope clearly and let it run asynchronously
- Start new users with easy, familiar tickets to build Devin's knowledge of the repo before scaling up
- Think about the future of software engineering by asking: what is the fundamental discipline (telling computers what you want), not what the current syntax is
- Take startup clichés literally; most founders know them but don't live them fully enough

### Notable Quotes
> "The soul of programming has really been about defining the problem that you're facing and really thinking through exactly what the solution you want to build."

> "I think there's going to be way more programmers and way more engineers a few years from now than there are today."

> "You want to be putting it all out on the field, but at the same time you want to be okay with both wins and losses."

> "It's often less about moats and more about stickiness."

## Sources
- [[scott-wu]] — "Inside Devin: The AI engineer that's set to write 50% of its company's code this year"

## See Also
- [[jevons-paradox-software]]
- [[ai-pair-programmer]]
- [[ai-non-determinism]]
- [[forward-deployed-engineer]]
