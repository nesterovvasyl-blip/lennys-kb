---
concept: Tactical vs. Strategic Retention
guests: [patrick-campbell]
topics: [retention, churn, saas, growth, product-management]
---

# Tactical vs. Strategic Retention

> Churn has two separate root causes — strategic (product/fit/value) and tactical (payment failures, cancellation flows) — but most product teams only address one and leave 25–40% of churn on the table.

## Overview

Patrick Campbell, founder of ProfitWell, developed this distinction from analyzing $30B+ in ARR through ProfitWell's platform. Most product teams are exclusively focused on strategic retention and systematically neglect tactical retention — a systematic mistake that typically accounts for 25–40% of total churn.

## Guest Perspectives

### Patrick Campbell ([[patrick-campbell]])

**Strategic retention** is everything product teams normally think about when they think about churn:
- ICP selection and fit — are you acquiring customers who will get lasting value?
- Time to value — how quickly do new customers experience the core benefit?
- Feature completeness — are you missing capabilities that cause people to leave?
- Pricing alignment — are customers paying commensurate with the value they get?
- Mission metric achievement — are customers reaching the key activation milestones?

This is the "product work" of retention. It requires excellent product strategy, roadmap prioritization, onboarding design, and customer success.

**Tactical retention** is everything product teams ignore because it doesn't feel like "product work":
- Payment failure recovery (dunning) — credit cards expire, get replaced, fail for reasons unrelated to intent to cancel
- Cancellation flows — the experience at the moment of cancel, before the decision is final
- Pause and maintenance plans — alternatives to full cancellation
- Offboarding — the experience after a customer decides to leave
- Term optimization — structuring billing cycles to reduce involuntary churn

Patrick analyzed two million cancellation flows and found specific patterns. You have 18-30 seconds when a customer hits "cancel":
- The optimal cancellation flow asks exactly two questions: "Why are you leaving?" (multiple choice, not free-form) and "What did you like about the product?" The second question activates nostalgia and interrupts the "freight train to cancel" mindset — buying time for a salvage offer or pause plan. It also provides valuable product signal.
- Free-form "why are you leaving?" responses are mostly noise — only 1% are usable signal. Multiple choice forces customers into categories that are actually analyzable.
- Based on responses + engagement data + plan data, a targeted offer (pause plan, retention discount, tier downgrade) can convert a cancellation into a save.

**Payment failure recovery**: Involuntary churn (failed credit cards, expired cards) is often 20-30% of all churn. Automated sequences with smart retry logic and dunning emails can recover a large fraction. ProfitWell offered this as a free product (Retain) — funded by the data they generated — because product teams would never prioritize building it themselves.

**Pause plans**: Offering a "pause" option before full cancellation — typically a 1-3 month pause at a reduced or zero rate — retains customers who have a temporary reason to leave (budget crunch, project pause) but would otherwise return. The salvage rate is significant.

### Why Product Teams Ignore This

Product teams are wired toward the future — new features, better UX, new ICPs. Tactical retention looks backward (why are people leaving today?) and operational (tune copy, add a flow, fix a payment processor). It doesn't feel like "building" — it feels like plumbing. Patrick's recommendation: assign tactical retention to the finance team, not product. Finance has the right incentives (revenue recovery) and won't deprioritize it in favor of roadmap work.

**The typical magnitude**: In Patrick's data across thousands of SaaS companies, tactical retention improvements alone reduced churn by 25–40% relative to baseline. At moderate scale, this is often worth more than months of product work.

## Actionable Takeaways
- Audit your cancellation flow: does it ask two questions (why leaving? + what did you like?) and offer a personalized salvage response?
- Measure your involuntary churn rate (payment failures) separately from voluntary churn — the interventions are completely different
- Build a dunning email sequence for failed payments that doesn't feel like a dunning email
- Consider creating a pause plan as an alternative to full cancellation
- Assign ownership of tactical retention explicitly — it often falls into no one's job description and dies

## Sources
- [[patrick-campbell]] — "10 lessons on bootstrapping a $200m business | Patrick Campbell (ProfitWell)"

## See Also
- [[freemium-subscription]]
- [[product-led-growth]]
- [[customer-led-growth]]
