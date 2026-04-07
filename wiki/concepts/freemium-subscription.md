---
aliases: [freemium, freemium-model, free-tier]
guests: [albert-cheng, patrick-campbell, oji-udezue]
---

# Freemium / Subscription

> A monetization model where a free tier drives adoption and a paid tier captures value — the conversion between them is the central product design challenge.

## Content

Freemium is a two-tier monetization structure: a free product available to all users, and a paid subscription (or one-time purchase) that unlocks additional value. The free tier drives acquisition and habit formation; the paid tier captures revenue from users whose engagement or needs exceed what the free tier provides.

The core design tension in freemium: the free tier must be valuable enough to attract and retain users, but constrained enough that a meaningful segment perceives sufficient additional value in the paid tier to convert. Both failure modes are common — free tiers so limited they fail to build habit (no conversion funnel), and free tiers so generous that users never perceive a reason to upgrade.

**Conversion patterns** are a major area of product experimentation in freemium products:
- **Time-limited trial**: Full access for N days, then cut off — creates urgency but breaks habit formation
- **Feature-gating**: Free tier has a subset of features; paid unlocks the rest — requires the gated features to be genuinely desirable
- **[[reverse-free-trial]]**: Premium features surfaced within the free experience up to a cap — exposure to value in context, not via countdown. [[albert-cheng]] reports Grammarly nearly doubled upgrade rates using this pattern.

Freemium works best when the product delivers immediate, perceptible value and the premium layer's benefit is qualitative and obvious at the moment of cap.

**Patrick Campbell's data on freemium vs. other acquisition methods** ([[patrick-campbell]]): Customers who convert from freemium have 10–20% higher retention than those converted from free trial or traditional sales. NPS for freemium-converted customers is roughly double. The explanation: freemium customers convert on their own timeline, not an artificial one created by a trial expiration or a salesperson. They've already internalized the product's value before paying. CAC has risen across SaaS channels, but freemium CAC has risen less than direct sales or paid channels — making it a relative bargain for middle-of-funnel conversion.

**Oji Udezue on freemium design** ([[oji-udezue]]): The critical design question is mandatory vs. optional onboarding. At Calendly, the mandatory onboarding (connect your calendar, set availability defaults) was short (two steps) and non-optional because those two actions set up all future success. Everything else — advanced configuration, templates, integrations — was optional and available for self-serve discovery. Splitting onboarding this way dramatically improves activation without overwhelming new users.

## Sources
- [[albert-cheng]] — referenced in context of Grammarly's upgrade rate improvements (Chess.com / Grammarly growth episode)
- [[patrick-campbell]] — "10 lessons on bootstrapping a $200m business | Patrick Campbell (ProfitWell)"
- [[oji-udezue]] — "Picking sharp problems, increasing virality, and unique product frameworks | Oji Udezue (Typeform)"

## See Also
- [[reverse-free-trial]]
- [[albert-cheng]]
- [[product-led-growth]]
