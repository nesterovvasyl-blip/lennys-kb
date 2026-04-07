---
author: archie-abrams
guests: [archie-abrams]
---
# Long-Term Holdout Experiments

> Shopify's method of holding experiment cohorts for 12+ months after shipping, to distinguish real long-term impact from short-term pull-forward effects.

## Content

Popularized (and practiced at scale) by [[archie-abrams]] at Shopify, long-term holdout experiments address a fundamental flaw in standard A/B testing: short-term lift metrics often don't predict long-term business outcomes.

### The Core Problem

Standard A/B tests measure impact over days or weeks. But many "wins" in that window are actually:
- **Pull-forward effects**: users activated sooner than they would have, but would have activated anyway — no incremental value created
- **False positives**: the metric being measured (activation rate, subscription rate) is not a good proxy for long-term GMV or revenue

Shopify's finding: **30–40% of short-term experiment wins show no meaningful long-term lift** on the metric that actually matters (cohort GMV over 3–5 years).

### Shopify's Two-Layer Holdout System

**Layer 1 — Global Quarterly Holdout**
5% of all users are held out of every new change shipped in a quarter. This bucket never sees new features. At the end of the quarter, comparing the holdout group to the rest shows the compound effect of all changes made in that period.

**Layer 2 — Cohort-Level Holdout**
For experiments that only affect new merchants, split 50/50 and run for a few weeks. Ship the winner to 100% — but keep tracking the original experiment cohort for 12 months. The experiment "result" is updated at 3, 6, 9, and 12 months automatically, creating an accountability ping for everyone involved.

### What the Data Shows

The most common outcome of long-term review is neutral — the short-term lift disappeared. The most common failure mode is the payment dunning example: sending better credit-card-failure reminders produced big short-term lift (more merchants saved), but at 6–12 months, GMV was flat because the merchants who let payments fail weren't deeply committed anyway.

The rare, valuable finding: pockets of merchants unlocked by a change who go on to build substantial businesses — often through **monetary friction reduction** (free trials, promotional credits, lower initial pricing).

### Why This Matters Beyond Shopify

Any company where the north star metric takes months or years to manifest — SaaS with long retention periods, marketplaces, consumer apps with purchase cycles — should consider holdout groups. The technique is practical: you ship the winner immediately (no delayed rollout), you just track the original cohort for longer.

### Implication: Absolute Numbers Over Conversion Rates

Long-term holdouts taught Shopify to optimize for **absolute numbers** (total merchants who reach X GMV) rather than conversion rates (% who activated). Conversion rates are optimizable by constricting the upstream funnel — a perverse incentive that destroys long-term value.

## Sources

- [[archie-abrams]] — "Look at experiments you thought were your biggest winners. Look at downstream metrics a year out. I'll bet you'd be surprised how many times the effect is different than you thought." (Shopify Growth)
- [[archie-abrams]] — "30–40% of things that show short-term lift probably don't have the same long-term impact. Most of the time it's actually a pull-forward." (Shopify Growth)

## See Also

- [[archie-abrams]]
- [[growth]]
- [[retention]]
- [[experimentation-culture]]
