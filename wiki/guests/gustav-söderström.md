---
guest: Gustav Söderström
role: Co-President & Chief Technology and Product Officer, Spotify
episode: "How Spotify builds product | Gustav Söderström"
date: 2023-09-07
topics: [product-development, ai-products, org-design, spotify, discovery, technology-strategy]
---

# Gustav Söderström

> Co-President and CPTO of Spotify, one of the most sophisticated thinkers on technology strategy, ML-driven product development, and organization design at scale.

## Content

Gustav Söderström is Co-President and Chief Technology and Product Officer at Spotify — one of the few leaders in tech who holds both the product and technology mandate simultaneously. He joined Spotify in its early days and has been central to the company's evolution from a music streaming service to a multi-format content platform. He is known for intellectual rigor, first-principles thinking, and a deep interest in how intelligence and technology interact.

### Key Ideas

- **Three eras of internet products — Curation → Recommendation → Generation**: Söderström's framework for understanding the history of internet product development. The first era was **Curation**: humans (editors, curators) decided what content was shown. The second era was **Recommendation**: ML systems replaced human curation using behavioral data. The third era, now beginning, is **Generation**: ML systems don't just recommend existing content but generate new content from a prompt or context. Spotify's homepage redesign story illustrates this progression — they moved from editorially curated playlists to algorithmic recommendations, and are now exploring generated mixes and summaries.

- **Fault-tolerant UI design**: One of Söderström's most actionable contributions to ML product thinking. The core insight: ML systems are probabilistic and make mistakes. UI design must match the actual hit rate of the underlying model. If a recommendation model is right 70% of the time, you need a UI that handles 30% wrong results gracefully — either by giving users easy correction mechanisms, by hedging the recommendation ("you might also like..."), or by showing multiple options. Building UI that assumes 100% accuracy on a 70%-accurate model creates a terrible product experience. The mismatch between expected and actual model accuracy is one of the most common ML product failures.

- **Abandoning the Squad Model**: Spotify famously pioneered the "squad model" of organization design (autonomous cross-functional teams, each owning their own product area). Söderström has said publicly that Spotify moved away from pure squad model at scale. The key tension: full squad autonomy is great for exploration and innovation, but it creates coordination failures when teams need to build on each other's infrastructure. The solution is a hybrid: autonomy at the VP level (strategic direction), centralization at the platform/infrastructure level.

- **Centralized (Apple) vs. Decentralized (Amazon) org models**: Söderström describes two archetypes of tech company organization. Apple's model: strong centralized product and design leadership, coherent aesthetic, tight integration — at the cost of speed in peripheral areas. Amazon's model: decentralized "two-pizza teams" with high autonomy — at the cost of inconsistency and duplication. Most companies sit on a spectrum and need to be intentional about where. Spotify has moved toward more centralization after experiencing the coordination costs of full decentralization.

- **10% planning time rule**: Söderström advocates that teams should spend approximately 10% of their working time on planning, strategy, and synthesis — not zero (which creates reactive chaos) and not 50% (which creates planning theater). The 10% figure is a useful default that forces both regular reflection and discipline against over-planning. He models this personally: he does regular walk-and-talk sessions to process strategic thinking.

- **Taste bubble and the discovery problem**: A deep insight about content recommendation: recommendation algorithms learn from what you've already chosen, which means they optimize for your revealed preferences in the past, not your potential preferences in the future. This creates "taste bubbles" — people get more of what they already like, but never discover what they would love if exposed to it. Spotify's homepage redesign was partly about breaking the taste bubble: showing things outside your typical patterns ("discovery mode") vs. giving you exactly what you've listened to before ("recall mode"). The tension is fundamental and unresolved.

- **Genetics to quantum to AI — magic until it's science**: Söderström's framing for how fields progress: everything that looks like magic eventually becomes science. Genetics was magic and art until it was science; quantum physics was mysterious until formalized; intelligence and creativity looked inexplicable until we had LLMs that describe them statistically. The practical implication: when something seems magical or inexplicable, push to formalize it. The inability to explain something is often just the absence of the right framework, not evidence of mystery.

### Actionable Advice

- When deploying ML in products: explicitly audit the expected accuracy of your model and then ask "Is our UI designed for this accuracy level?" If the model is wrong 30% of the time, you need design that handles 30% errors.
- Teams spending zero time on strategy and planning are as broken as teams spending too much. Default to 10% of time on synthesis/planning.
- Don't assume the squad model is right for your organization. Evaluate: what needs coherent central vision (design, platform infrastructure) vs. what benefits from autonomous exploration?

### Notable Quotes

> "Genetics was magic and art until it was science. Intelligence and creativity were magic until they were statistics in an LLM."

> "If your recommendation model is right 70% of the time, your UI must be designed for 30% errors. Otherwise you've built a product for the wrong model."

> "Spotify pioneered the squad model and then we moved away from it. Full autonomy is great until you need things to work together."

## Sources
- [[gustav-söderström]] — "How Spotify builds product" (2023)

## See Also
- [[fault-tolerant-ui-design]]
- [[curation-recommendation-generation]]
- [[org-design]]
- [[ai-products]]
- [[spotify]]
