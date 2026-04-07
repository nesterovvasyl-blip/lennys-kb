---
guest: Jason Droege
role: CEO, Scale AI; former founder of Uber Eats
episode: "Scale AI CEO on Meta's $14B deal, scaling Uber Eats to $80B, & what frontier labs are building next"
date: 2025-10-09
topics: [ai-training-data, growth, strategy, leadership, hiring, startup-lessons, product-market-fit, innovation]
---
# Jason Droege
> CEO of Scale AI and the person who built Uber Eats from an idea to a multi-billion dollar run rate business — with a philosophy of independent thinking, incentive-mapping, and an unrelenting bar for what makes a business worth building.

## Content

Jason Droege co-founded Scour (a peer-to-peer file-sharing network) with Travis Kalanick while students at UCLA in the late 1990s — learning at 19 that "everything is negotiable" when their investors kept moving the terms, and then watching the company be sued for a quarter of a trillion dollars before settling for $1 million. He then built Uber Eats from scratch inside Uber, growing it to an $80B+ run rate business that kept Uber alive during COVID when ride-sharing collapsed. He became CEO of Scale AI 13 months before the time of recording, taking over after the Meta deal (Meta invested $14B for 49% non-voting stock; Alex Wang moved to Meta's superintelligence team).

### Key Ideas

- **The data labeling evolution**: Scale was founded on the insight (from a 19-year-old Alex Wang) that data was the bottleneck to better models. The business evolved through three phases: (1) autonomous vehicles computer vision labeling, (2) GenAI text tasks (short stories, preference ranking), (3) expert tasks that take hours and require PhDs — e.g., building an entire website with reasoning annotations, explaining nuanced cancer treatments to a model. 80% of Scale's expert network has a bachelor's degree or higher; ~15% have PhDs.

- **From knowing to doing**: The general trend in AI models is the shift from "models knowing things" to "models doing things." This requires RL environments — sandboxed contexts where AI agents can practice navigating real systems (Salesforce instances, healthcare records, calendar apps) and learn from failure. These environments are highly non-generalizable: the same task type in different enterprise configurations requires different training data, because organizational context and judgment patterns differ company to company.

- **Digitizing human judgment**: The bottleneck for enterprise AI is not generic intelligence but domain-specific judgment — how does *this doctor at this hospital* make decisions given *this institution's* culture, protocols, and patient population? Off-the-shelf models plus RAG plus fine-tuning gets you most of the way, but the last mile requires the specific experts at the specific organization to do their own labeling. Scale calls this "digitizing judgment."

- **AI enterprise reality vs. hype**: Real, robust enterprise AI implementations take 6–12 months to get to production quality. POCs get to 60–70% accuracy quickly, but the gap from there to reliability is exponential (like data center uptime: each nine is an order-of-magnitude investment). The 95% failure rate of enterprise AI pilots is partly misleading — it reflects how easy it is to *start* a project, not how hard it is to finish one well.

- **Entrepreneurship as alpha-seeking**: Droege's framework for founders: why do you have an insight that others don't? Given millions of smart people trying things, what makes you specifically likely to have a non-consensus view that turns out to be correct? His answers: you're in a "narrow, far-flung place" that gives you unusual vantage, or you're constitutionally contrarian. The second test: why do you want to work on this for 5–10 years? The urgency question — not "does the customer have a problem" but "is this problem urgent enough to them right now?" — is what most founders miss.

- **Understanding customer incentives, not just pain**: When Droege was building Uber Eats, restaurant owners would list many problems (labor costs, ingredients costs). But their daily urgency was simpler: did I make money yesterday, will I make money tomorrow? The real insight was incremental demand economics: a restaurant's ingredient cost is 20–30% of revenue, labor 20–30%, but incremental orders on existing staff have 70–80% gross margin. That math justified Uber's 30% commission in a way that "we'll help you with ingredients" never would have.

- **Good markets vs. bad markets**: The filter Droege applies to any new business idea: is this a marketplace, SaaS, recurring revenue, network-effects, or lock-in business? Businesses that are more valuable at scale than at small scale are the ones worth the effort. Most ideas fail this filter quickly. What's left gets evaluated on passion and insight quality.

### Actionable Advice

- Before talking to customers, map their incentives — financial, career, ego — not just their stated pain. The urgency of the problem (is this top of mind daily or annually?) is as important as the problem's size.
- Decompose your own ground truth independently before relying on what customers tell you. Uber Eats literally weighed ingredients to verify restaurant economics before designing the commission structure.
- For AI products: do not confuse POC success with production readiness. Budget 6–12 months and plan for each reliability "nine" to be an order-of-magnitude more expensive than the one before.
- To find your startup insight: ask not "is there a problem here" but "why am I the person who sees this clearly, and why now?"

### Notable Quotes

> "From an entrepreneurship standpoint, it truly is about what insight do I have? Why in a world of a million entrepreneurs who are thinking, who are smart, who are trying everything, why am I in the position where I likely have an insight that others do not?"

> "Things take 6 to 12 months to get truly robust enough where an important process can be automated. Easy to learn, hard to master."

> "A good business is more valuable at scale than at small scale — network effects, lock-in, recurring revenue. Everything else fails the filter pretty fast."

> "Everything is negotiable. There is no way to do things. There is just the way that you can negotiate your way through the world."

## Sources
- [[jason-droege]] — "Scale AI CEO on Meta's $14B deal, scaling Uber Eats to $80B, & what frontier labs are building next"

## See Also
- [[ai-training-data]]
- [[ai-evals]]
- [[rl-environments]]
- [[strategy]]
- [[startup-resilience]]
