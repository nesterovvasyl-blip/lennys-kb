---
aliases: [freemium, freemium-model, free-tier]
guests: [albert-cheng, naomi-ionita, patrick-campbell]
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

## Guest Perspectives

### Albert Cheng

Albert Cheng at Grammarly used a [[reverse-free-trial]] pattern — surfacing premium features within the free experience up to a cap — and nearly doubled Grammarly's upgrade rates.

### Naomi Ionita

Naomi Ionita's Evernote experience is the definitive cautionary tale in freemium design. At $45/year with no segmentation, surveys revealed that the top upgrade motivator was *guilt* — users felt obligated to pay for something they used so much. If guilt is a primary conversion driver, the free tier is too good.

The fix Naomi advocates: **bifurcate tiers based on user journey stage**. "Day one features" (the path to the aha moment, habit formation) belong in the free tier — without them, you collapse time-to-value and break the funnel. "Day 100 features" (advanced functionality whose value emerges with scale, collaboration, or history) belong in paid tiers. At Invoice2go, applying this framework doubled upgrade rates from starter to pro *while simultaneously raising the pro price 30%*.

Additional Evernote failure mode: Evernote was philosophically antisocial (designed as a personal "second brain"), which made it nearly impossible to retrofit collaboration. The result: it capped out as a prosumer tool and never crossed into enterprise. Contrast with Notion, which was collaboration-first from day one. Naomi's principle: **you can't retrofit collaboration**.

On free tier math: free users who don't directly pay still have value — they drive organic acquisition (referrals, shared workflows) and reduce CAC. The free tier is a growth investment, not just a conversion funnel.

### Patrick Campbell

Campbell argues freemium is one of the most underutilized tools for building middle-of-funnel momentum. Most sales and marketing budgets go to top-of-funnel (awareness) and bottom-of-funnel (closing), with almost nothing in the middle. Freemium fills this gap: it creates a pool of users who are aware of your product, using it, and waiting for the right moment to convert — on their own timeline.

Key data from ProfitWell's dataset of $30B+ in subscription ARR:
- Customers who convert from freemium have 10-20% higher retention than those who convert from free trials or traditional sales
- NPS/CSAT for freemium converts is approximately double vs. other acquisition paths (they convert voluntarily, not under artificial deadline pressure)
- CAC for freemium acquisitions has grown much more slowly than overall CAC over the past decade

His reframe: freemium is not just a conversion mechanism — it's a demand-generation channel. The free product is better content than any blog post or webinar, because customers are using the actual product and telling colleagues about it.

Campbell is a convert; he previously wrote articles arguing freemium was bad. His current view: it's one of the most powerful tools available, especially in a world of rising CAC and increasing competition.

## Sources
- [[albert-cheng]] — referenced in context of Grammarly's upgrade rate improvements (Chess.com / Grammarly growth episode)
- [[naomi-ionita]] — Evernote pricing experience, day-one vs. day-100 feature framework, Invoice2go pricing restructure (How to price your product)
- [[guests/patrick-campbell]] — 10 lessons on bootstrapping a $200m business

## See Also
- [[reverse-free-trial]]
- [[albert-cheng]]
- [[naomi-ionita]]
- [[concepts/product-led-growth]]
