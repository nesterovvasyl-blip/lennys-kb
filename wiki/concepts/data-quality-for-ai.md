---
concept: Data Quality for AI Products
guests: [shaun-clowes, scott-wu]
topics: [ai-products, product-management, data-strategy, saas-defensibility]
---

# Data Quality for AI Products

> The value of an AI-powered product is determined almost entirely by the quality, freshness, and relevance of the data fed to the model — not by the model itself.

## Overview

As AI products proliferate, a common misconception is that the primary differentiator is model capability. Multiple guests on the podcast argue that data — its quality, timeliness, relevance, and the infrastructure to continuously deliver it to the model — is the real differentiator. Models are commoditizing; data systems are where the long-term advantage lives.

## Guest Perspectives

### Shaun Clowes ([[shaun-clowes]])

Clowes' central AI thesis for CPOs: LLMs are "information shredders" — they can process unlimited information, and the more high-quality, timely, relevant data you give them, the better they perform. The constraint is never the model; it's the data.

**Information decay rate:** Customer feedback, competitor positioning, and market conditions all age quickly. An LLM trained on stale context will produce stale output, no matter how smart the underlying model. This makes data pipeline freshness a core product engineering problem.

**The 90% problem:** Teams think they can build great AI by wiring in a model and a basic data pipeline. In practice, 90% of the calories go to data management — getting access to good data, high-quality data, timely data, well-structured data, and getting it to the LLM context at the right time.

**Implication for SaaS defensibility:** The hardest-to-copy moat in B2B SaaS is the accumulated business rules — years of customer-specific configuration in applications like Salesforce or Workday. This same principle applies to AI products: the company with the best proprietary data about a specific domain (accumulated over years through customer usage) will build AI features that competitors can't replicate quickly.

**Practical use for PMs:** When using AI for product analysis — customer interviews, competitor research, strategy documents — always push toward disconfirmation. Ask the model where your strategy *doesn't* fit customer feedback, not where it does. Ask it whether competitor positioning fits your customers better than your own. The value is finding gaps, not confirming assumptions.

### Scott Wu ([[scott-wu]])

Wu makes a complementary point from the engineering perspective. Devin's competitive advantage is not just the model intelligence — it is the accumulated knowledge of your specific codebase built up over time through usage. The longer your team uses Devin and the more it learns about your stack, processes, and patterns, the harder it becomes to replicate that value with a fresh agent.

Wu's framing: teaching the AI what there is to know about your codebase is an ongoing investment. Switching to a new agent means starting over — that is the real stickiness.

## Actionable Takeaways
- Evaluate AI products on data infrastructure first: what data does it have access to, how fresh is that data, how does it accumulate over time?
- When building AI features, invest heavily in data pipelines before model integration
- Use AI to find disconfirmations (where is my strategy wrong?) not confirmations
- Long-term AI product defensibility comes from proprietary data accumulation, not model access
- For product managers using AI in research: put all available context (transcripts, competitor docs, survey data) into the LLM before asking questions — the model is only as useful as what you give it

## Sources
- [[shaun-clowes]] — "Why great AI products are all about the data"
- [[scott-wu]] — "Inside Devin: The AI engineer that's set to write 50% of its company's code this year"

## See Also
- [[ai-training-data]]
- [[context-engineering]]
- [[ai-evals]]
- [[jevons-paradox-software]]
