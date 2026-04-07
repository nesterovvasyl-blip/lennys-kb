---
guest: Guillermo Rauch
role: Founder & CEO, Vercel; Creator of Next.js, Socket.IO
episode: "Everyone's an engineer now: Inside v0's mission to create 100 million builders"
date: 2025-04-13
topics: [ai-products, developer-tools, product-development, taste, design, future-of-work]
---

# Guillermo Rauch

> Founder and CEO of Vercel, creator of foundational JavaScript frameworks Next.js and Socket.IO, and the mind behind v0 — the AI-powered web builder aiming to expand the universe of people who can ship software from 20M to 100M.

## Content

Guillermo Rauch has been building foundational developer infrastructure for over a decade. He created Socket.IO (the real-time communication engine powering Notion, among others) and Next.js (the React framework underlying Claude, Grok, Midjourney, and thousands of other products). Vercel, the company he founded, serves as the deployment and infrastructure platform for much of the modern web. His latest bet is v0, an AI-powered web builder that turns text prompts and screenshots into production-ready code — with the ambition of reaching the 100 million people who want to build digital products but couldn't before.

### Key Ideas

- **TAM expansion through democratization**: v0's strategic logic is expanding the total addressable market for Vercel. Vercel had ~5M React developers and ~20M JavaScript developers as its potential users. Guillermo's hypothesis: there are ~100M people who want to build and ship digital products. v0 removes the translation barrier between intent and implementation, making Vercel's infrastructure accessible to non-engineers. The TAM expansion and the distribution/UX revolution are the same bet.

- **AI as software — stop talking about AI**: Guillermo's provocative framing: "I just see a future where AI becomes synonymous with software. We build software and we use software to build software." The "AI" framing is temporary; eventually the distinction dissolves. Products will just be... better. Faster. More responsive to intent. The framing shift has practical implications: stop treating AI features as a separate category and integrate them into the core product loop.

- **The future of skills — knowing how things work, not memorizing syntax**: Guillermo's children framework for "what should my kids learn": math (logical reasoning), eloquence (linguistic precision, the ability to steer models), and understanding of how things work (conceptual knowledge of systems, not encyclopedic memorization). The professional CSS expert who knows every property by heart is being replaced by v0; the person who understands layout systems conceptually and can say "turbulence" or "neobrutalist" to steer the model is not.

- **Translation tasks are going away; judgment remains**: Programming roles that were fundamentally translation tasks — converting a design screenshot into CSS/React implementation — are being automated. What persists is judgment: knowing what to build, why, and whether the output is actually good. Guillermo's test: he replicated his own personal website using v0 and it took 10 prompts in the previous model generation, 2 prompts in the latest. The model also produced more accessible code than he wrote himself.

- **Increasing exposure hours**: Taste is a learnable skill, not a birthright. Guillermo's internal Vercel operating principle: measure and maximize "exposure hours" — time spent watching users interact with your product, using competitive products, attending user interviews. The more exposure hours an engineer or designer has, the better their product instincts become. He runs regular customer demos at executive team meetings and Demo Fridays so everyone sees real usage.

- **Escape hatches in system design**: Inspired by React's design principle, Guillermo argues every AI tool (and every product system) should provide an escape hatch — a way to get out of the guardrails and work directly with the underlying layer. For v0, this means always showing the generated code and allowing direct editing. The escape hatch is what makes the tool trustworthy and extensible for power users.

- **Social product building**: Guillermo frames v0 Community (a GitHub-like fork/share system for v0 projects) as "social product building" — the successor to GitHub's social coding. GitHub democratized code-sharing but required knowing how to code. v0 Community democratizes product-sharing. Within weeks of launch it had 20,000 submissions with thousands of forks.

- **Tight user feedback loops**: The key product principle Guillermo credits for Vercel's success: build mechanisms for users to give you feedback at the moment of frustration or delight. Vercel's early feedback button sent responses directly into Slack, creating a real-time stream of user sentiment that shaped every product iteration.

### Actionable Advice

- For product builders: measure exposure hours. How many hours this week did you watch users actually use your product? Track it and increase it deliberately.
- When building with v0 or any AI tool: give it inspiration and references ("make it look like Charles Schwab," "use turbulence for the animation"), not just functional requirements. The model knows the tokens.
- For AI products: add user feedback mechanisms that reach builders directly (not just a support ticket queue). The feedback loop velocity is a competitive moat.
- "Just try something else" — when an AI tool is stuck, don't debug; redirect. Reframe the prompt, suggest a different approach, and it often unsticks.

### Notable Quotes

> "v0 is like a super genius five-year-old PhD with ADHD. It knows everything about everything, but it has these sparks of brilliance."

> "We need to stop talking about AI at some point. AI becomes synonymous with software. We build software and we use software to build software."

> "Taste is a skill that can develop. Increase exposure hours — quantify how much time you expose yourself to watching people use your products."

> "I want to find the thing v0 cannot build. So far I'm still looking."

## Sources
- [[guillermo-rauch]] — "Everyone's an engineer now: Inside v0's mission to create 100 million builders" (2025)

## See Also
- [[ai-products]]
- [[developer-tools]]
- [[design-taste]]
- [[future-of-software-development]]
