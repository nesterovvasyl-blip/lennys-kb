---
author: Itamar Gilad
guests: [itamar-gilad]
---
# Confidence Meter
> A calibration tool for product teams that assigns honest confidence scores (0–10) to ideas based on the type of evidence supporting them — preventing the cognitive bias of inflating confidence when the only backing is opinion.

## Content

Created by Itamar Gilad as part of the [[gist-model]], the confidence meter solves a specific problem with ICE scoring: people systematically inflate the "C" (Confidence) component when their evidence is weak. An idea with a compelling pitch deck and a loud sponsor gets scored 8/10 confidence — not because the evidence is strong, but because the presenter *feels* strongly about it.

The meter works like a thermometer, ranging from 0 (no evidence, pure speculation) to 10 (fully validated, launched, proven). Across the dial, it maps classes of evidence to specific confidence ranges:

**Blue zone (low confidence — 0 to ~3):**
- Self-conviction / personal enthusiasm: ~0.01
- Pitch deck or six-pager: ~0.1
- Thematic support ("it's about AI"): ~0.1
- Stakeholder review: ~0.5–1
- Business modeling / back-of-envelope calculation: ~1

**Orange zone (medium confidence — 3 to ~6):**
- Anecdotal data points from existing datasets: ~2
- User interviews (handful): ~3
- Competitive analysis: ~3
- Market surveys: ~4–5
- Expert opinion (external domain experts): ~4

**Red zone (high confidence — 6 to 10):**
- Fake door / smoke tests: ~6
- Wizard of Oz / concierge tests: ~6
- Usability studies with prototypes: ~7
- Early adopter programs / alphas: ~7
- AB test (randomized, controlled): ~8–9
- Staged rollout with holdback group: ~9–10

**How to use it:**

When evaluating an idea in ICE scoring, ask: "What's the actual evidence we have for this impact estimate?" Then locate that evidence on the meter to get an honest confidence score. If the answer is "we believe it strongly and our VP likes it," the confidence score is 0.1 — which should change how much you're willing to invest before validating further.

The meter also guides *investment proportional to confidence*: low confidence → cheap validation experiments first. High confidence → commit to full build. You don't have to climb the whole meter — some ideas are low-risk enough that you can skip to AB test directly.

**Common misuse:**

Teams sometimes use the confidence meter as a bureaucratic gate rather than a calibration tool, requiring high confidence before any experimentation. This is the opposite of the intent. The meter helps you *start* experiments at the right fidelity for your current confidence level — not to delay until you're confident.

## Sources & See Also
- [[itamar-gilad]] — "Becoming evidence-guided" (Lenny's Podcast); *Evidence-Guided* (book)
- [[gist-model]]
- [[experimentation-culture]]
- [[product-market-fit]]
