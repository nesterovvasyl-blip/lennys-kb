---
aliases: [fault-tolerant-ui-design, ml-ui-accuracy-matching]
guests: [gustav-söderström]
---

# Fault-Tolerant UI Design

> The principle that ML-powered product UI must be designed to match the actual accuracy of the underlying model — not assumed perfect accuracy. If the model is right 70% of the time, the UI must gracefully handle 30% errors.

## Content

Articulated by [[gustav-söderström]], CPTO of Spotify, based on learnings from building recommendation-driven products at scale.

**The failure mode**: A team builds a recommendation model with 70% accuracy. The UX team designs a UI assuming the model is always right — prominent placement, no alternatives shown, no easy correction. The result: users are confused or frustrated 30% of the time, blame the product, and churn. The engineers say "the model is pretty good." The PMs say "users hate it." Both are right; the disconnect is the UI's implicit assumption about model accuracy.

**The principle**: UI design is not separate from model design — it must be calibrated to the model's hit rate. If a content recommendation is right 95% of the time, you can make it prominent and default. If it's right 60% of the time, you need multiple options, easy skipping, or hedged language ("you might also like..."). If it's right 40% of the time, you shouldn't be surfacing it as a primary recommendation at all.

**Practical applications at Spotify**:
- Playlist recommendations: when confidence is high (based on strong behavioral signals), show one clear recommendation. When confidence is lower (new user, unusual taste), show multiple options.
- Discovery vs. recall modes: the homepage shows different UI depending on whether Spotify is confident you want something familiar (high confidence recall) or is suggesting you explore (lower confidence discovery). The UI explicitly signals uncertainty in discovery mode.

**The broader principle**: As ML systems are deployed more broadly in products, UI designers and product managers need to think in probability distributions, not binary outcomes. Features are not "working" or "not working" — they're working X% of the time, and the product experience should reflect that distribution.

**Relationship to trust calibration**: Users develop trust in AI-powered features based on their experience. A feature that's right 95% of the time with a UI designed for 95% accuracy will be trusted. The same feature with a UI designed for 100% accuracy will be distrusted because the failures feel jarring and unexpected. Fault-tolerant UI manages the failure expectation explicitly.

**Design patterns**:
- Show confidence signals (lighter text, hedged language, "might", "based on your recent listening")
- Provide easy escape hatches (skip, "not interested," explicit alternatives)
- Avoid hiding alternatives when model confidence is below ~85%
- For high-stakes predictions, show multiple options ranked by confidence, not a single "answer"

## Sources
- [[gustav-söderström]] — "If your recommendation model is right 70% of the time, your UI must be designed for 30% errors." (How Spotify builds product, 2023)

## See Also
- [[gustav-söderström]]
- [[ai-products]]
- [[curation-recommendation-generation]]
