---
concept: Overall Evaluation Criterion (OEC)
guests: [ronny-kohavi]
topics: [experimentation, metrics, ab-testing, product-development]
---

# Overall Evaluation Criterion (OEC)

> The single composite metric (or constrained metric system) that an experiment must move to justify shipping — designed to be causally predictive of long-term user value, not just short-term business outcomes.

## Overview

The OEC is one of the most important and most commonly overlooked elements of a mature experimentation program. Most teams start with an obvious metric — revenue, conversion rate, time on site — but quickly discover that optimizing these directly leads to poor outcomes for users and the long-term business.

The OEC solves this by requiring that the metric:
1. Be **causally predictive of lifetime value** — improving it must genuinely make users better off over time, not just spike a short-term number
2. Include **countervailing guardrail metrics** — so you can't improve the primary metric by degrading user experience
3. Be **directionally agreed upon** — everyone on the team must agree that "more is better" (or "less is better"), otherwise the OEC is useless

## Guest Perspectives

### Ronny Kohavi ([[ronny-kohavi]])

Kohavi developed the OEC concept through repeated failures across Amazon, Microsoft/Bing, and Airbnb — each case illustrating what happens when teams optimize for incomplete metrics.

**Bing Ads example**: Optimizing for revenue-per-search encourages adding more ads to every page. This increases short-term revenue but damages user experience and increases churn. The fix: frame the optimization as a constraint — "maximize revenue *per pixel of ad space*" — so expanding ad real estate requires a higher revenue-per-pixel, not just more pixels. This prevented the "add more ads" local maxima.

**Amazon email recommendations example**: When the email team measured success by "revenue from clicks that came through email," the team scaled spam — more emails meant more revenue attribution, regardless of whether those emails were helpful. The fix: model the dollar cost of unsubscribes (future lost email revenue), subtract from revenue attribution. Once this was included, more than half of active campaigns were net-negative. The OEC restructured incentives from "send more" to "send better."

**Airbnb booking example**: Conversion rate is the wrong OEC for bookings. It can be improved by surfacing cheaper listings that people will regret. A better OEC includes the post-stay review rating — predicting (via a model trained on historical data) whether the user will be happy with the booking months later.

**The microsoft.com counterexample**: A team at Microsoft proposed "time on site" as their OEC. Ronny asked: is more time on site good (users are engaged) or bad (users can't find what they want)? Half the room said good, half said bad. An OEC where the team can't agree on the direction is not an OEC — it's a measurement with no strategic implication.

## Actionable Takeaways
- Before launching any experiment program, define your OEC with the entire team until everyone agrees on direction
- Ask: "Can someone improve this metric while making users worse off?" If yes, you're missing a guardrail metric
- Frame OEC as causally predictive of lifetime value, not just immediate revenue or engagement
- Use constraint optimization framing when primary and secondary metrics conflict: "maximize X subject to Y not decreasing more than Z"
- When you can't measure the true long-term metric directly, build predictive models using historical data (e.g., early booking signals that predict review satisfaction)

## Sources
- [[ronny-kohavi]] — "The ultimate guide to A/B testing | Ronny Kohavi (Airbnb, Microsoft, Amazon)"

## See Also
- [[experimentation-culture]]
- [[long-term-holdout-experiments]]
- [[ab-testing-principles]]
