---
aliases: []
episode_title: "How Community Notes works — and why it's the most important product in tech"
publish_date: 2025-02-27
youtube_url: https://www.youtube.com/watch?v=8dgyqYHLcCI
topics: [trust-and-safety, misinformation, crowdsourcing, content-moderation, ai-products]
---

# Keith Coleman & Jay Baxter

> Keith Coleman is VP of Product at X (Twitter). Jay Baxter is the lead researcher behind the Community Notes algorithm. Together they built Community Notes — Twitter/X's crowdsourced fact-checking system.

## Bio

Keith Coleman is VP of Product at X. Jay Baxter is the researcher and engineer who designed the algorithmic core of Community Notes. Their episode is a deep technical and philosophical dive into how Community Notes works, why it was designed around cross-partisan agreement rather than majority vote, and why they believe it represents the future of trust and safety at scale.

## Key Ideas

### Bridging-Based Agreement Algorithm

Community Notes rejects the obvious approach (majority vote on whether a note is helpful) because majority vote would mean partisan majorities could systematically suppress accurate corrections to misinformation that their side prefers. Instead, Community Notes uses a **bridging-based algorithm**: a note only becomes visible if it receives helpful ratings from people who typically disagree with each other. Cross-partisan agreement is the quality signal.

The algorithm maps each contributor on a political spectrum based on their rating patterns, then surfaces notes that received positive ratings from people across the spectrum. This means a note about a conservative tweet must get helpful ratings from both conservatives and liberals to appear — and vice versa.

### Why This Design

The insight: misinformation often spreads along partisan lines. If you allow the majority to determine what's "misinformation," you get weaponized fact-checking — each side flags the other's content. Cross-partisan agreement is a more robust signal for truth than any single community's consensus.

This is a fundamental philosophical choice: optimize for accuracy over speed, and for legitimacy over volume.

### Scale and Adoption

- 950,000 contributors globally
- 30 billion note views in 2024
- Now being adopted by Meta (Facebook/Instagram) as the model for their fact-checking replacement

The fact that Meta adopted the Community Notes model is significant — it suggests the bridging-based approach is becoming the industry standard for crowdsourced content moderation.

### Open Source Transparency

The algorithm is fully open source. Anyone can download the data and run the algorithm themselves to see which notes are rated helpful. This transparency is core to the legitimacy of the system — contributors can verify the system isn't biased against them.

### Limits and Failure Modes

Community Notes does not catch everything. It works best on specific factual claims that can be verified. It struggles with:
- Nuanced or contextual misinformation
- Fast-moving breaking news (notes take time to be written and rated)
- Content where there's genuine expert disagreement

The system is not designed to moderate all harmful content — only to add context to misleading content when contributors can agree.

### Product Philosophy

Keith and Jay articulate a philosophy for trust and safety products: if you want scale, you need community. Professional fact-checkers can't review billions of posts. Algorithms alone are too blunt and gameable. The synthesis is a community-powered system with algorithmic backbone — human judgment operating at machine scale.

## Memorable Quotes

- "The insight was: if people who normally disagree with each other agree that a note is helpful, that's a much stronger signal than majority agreement."
- "We open-sourced the algorithm so anyone can check our work. Transparency is part of the legitimacy."
- "We're not trying to moderate everything. We're trying to add context when that context is verifiable and cross-partisan."

## Actionable Advice

- When designing crowdsourced systems, choose your agreement signal carefully — majority vote is gameable by the largest group
- Transparency (open source data + algorithm) is a trust feature, not just a technical nicety
- For trust and safety at scale, think community + algorithm, not either/or

## Topic Tags

trust-and-safety, content-moderation, crowdsourcing, misinformation, bridging-based-agreement, community-notes, open-source

## See Also

- [[community-notes]] — dedicated concept page
- [[kevin-weil]] — also worked at Twitter/X on product
