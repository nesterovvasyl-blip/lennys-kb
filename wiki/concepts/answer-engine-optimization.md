---
aliases: [aeo, geo, generative-engine-optimization, llm-seo]
guests: [ethan-smith]
---

# Answer Engine Optimization (AEO)

> The practice of optimizing content to appear as a cited source in LLM-generated answers — the emerging complement to traditional SEO for an era when people ask AI assistants instead of search engines.

## Content

Answer Engine Optimization (AEO) — also called Generative Engine Optimization (GEO) or LLM SEO — is the discipline of ensuring your content appears when users query ChatGPT, Perplexity, Gemini, or Claude about topics relevant to your product. The most comprehensive treatment in the Lenny's Podcast canon is from Ethan Smith (CEO, Graphite), who has conducted rigorous empirical research on what works.

### The Core Mechanism: LLM + RAG

AEO is not about getting into model training data. LLMs use Retrieval-Augmented Generation (RAG): when a user asks a question, the model queries the web, retrieves relevant pages, and summarizes those pages. AEO means getting your content into those retrieved pages and cited in the summary.

This makes AEO fundamentally similar to SEO, not a replacement for it. The same authority signals matter, the same content quality principles apply, and the same link graph influences rankings — but the surface (an LLM summary with citations) is different from ten blue links.

### Key Metrics: Share of Voice

Unlike traditional SEO (rank #1 for keyword), AEO success is measured as "share of voice" — the percentage of the time your brand or content is cited across a sample of relevant questions on a given platform. Because LLMs return different answers to the same question each time (probabilistic), you need to ask each question multiple times and measure your citation rate.

### The Long Tail Opportunity

Average Google query: 4-6 words. Average ChatGPT question: 20-25 words. The tail of questions people ask in LLMs is vastly larger than in traditional search, because conversational queries have no upper bound on specificity. Most of this tail is uncontested — no company has optimized for "which payroll software integrates with Looker via Zapier and outputs to BigQuery?" A help center article that answers this exactly may be the only citation available.

### Citation Optimization Strategy

Smith breaks AEO offsite strategy into source tiers:

| Source | Effort | Control | Best For |
|--------|--------|---------|----------|
| Affiliate publishers (Dotdash, Forbes) | High cost | High | B2C, high-competition keywords |
| YouTube/Vimeo | Low-medium | High | B2B (almost no competition) |
| Reddit | Low | Low (community decides) | Authentic, long-tail |
| Your own landing pages | Medium | High | Topic clusters |
| Help center | Low (existing content) | High | Feature/use-case questions |

### Help Center Optimization

An underused AEO tactic: optimize your help center. Most companies have help centers that cover head questions but miss the long tail of "can you do X?" queries. Specific fixes:
1. Move from subdomain (help.company.com) to subdirectory (company.com/help) — subdirectories perform better
2. Add cross-links between help pages
3. Create pages for long-tail use cases surfaced from sales calls and customer support

### B2B vs. B2C Differences

For B2B: citations are typically niche trade publications (TechRadar, etc.), not consumer media. Impact is mostly non-clickable (users read the answer, then open a new tab and search for the brand name directly). Measurement requires brand search tracking and post-conversion surveys, not just referral traffic.

For commerce/B2C: LLMs are adding shoppable cards (like Google Shopping). Click-through rates are higher. Schema markup and review counts matter more.

### AI Content Does Not Work

Empirical finding from Graphite's research: only 10-12% of pages cited by Google and LLMs are AI-generated. Fully automated AI content is systematically excluded. Human-edited AI-assisted content works fine. The reason: LLMs trained on AI derivatives experience "model collapse" — converging on a single opinion rather than reflecting the diversity of human knowledge. Google and LLM systems detect and penalize this.

### SEO Is Not Dying

Despite hype, Google organic traffic is not declining — it's slightly up per Google's own VP of Search. LLMs are an additive channel, not a substitute. Both should be invested in.

### Webflow Case Study

Webflow integrated AEO into their growth strategy. Results at time of recording:
- 8% of all new signups from LLM-referred traffic
- 6X conversion rate vs. Google organic traffic (higher intent users)
- LLM is now a top acquisition channel, comparable to paid

## Sources
- [[ethan-smith]] — "AEO is LLM plus RAG. You're not trying to get into the model's weights. You're trying to get cited in the search results that the model uses to answer." (A complete guide to Answer Engine Optimization)

## See Also
- [[ethan-smith]]
- [[seo]]
- [[marketing]]
- [[growth]]
- [[content-strategy]]
