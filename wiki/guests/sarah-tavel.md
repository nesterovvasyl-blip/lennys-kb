---
guest: Sarah Tavel
role: General Partner, Benchmark (formerly Partner, Greylock; first PM at Pinterest)
episode: "The hierarchy of engagement | Sarah Tavel (Benchmark, Greylock, Pinterest)"
date: 2023-12-27
topics: [consumer-products, marketplaces, growth, retention, engagement, product-strategy, venture-capital]
---

# Sarah Tavel

> General Partner at Benchmark (boards: Chainalysis, Hipcamp, Rekki, Cambly, Medely), founding member of All Raise, and the first product manager at Pinterest — Sarah thinks like a PM even as a VC, with a strong allergy to vanity metrics.

## Background

Sarah was Pinterest's first product manager, leading the discovery team (home feed, search, recommendations). She then joined Greylock as a partner before moving to Benchmark, one of the most prestigious early-stage VC funds. She also played rugby and was "one of the best tacklers in the league." At Benchmark, she focuses on consumer and marketplace startups at the Series A stage.

This episode covers two of her most influential frameworks: the Hierarchy of Engagement and the Hierarchy of Marketplaces.

---

## Framework 1: The Hierarchy of Engagement

See also: [[hierarchy-of-engagement]]

Sarah's framework for building enduring consumer products. Developed as a reaction against MAU-obsessed growth hacking, it asserts that **engagement, not acquisition, is the foundation of a lasting consumer business.**

### Level 1: Core Action

Every product has one action that serves as its foundation. When a user completes this action, they:
- Understand what the product is for
- Are highly likely to return

Examples:
- Pinterest → pinning/repinning
- Facebook (early) → friending
- YouTube → subscribing (not watching — per Shishir Mehrotra's correction)
- Snapchat → sending a snap
- Evernote → writing a note

Key nuance: **activation milestone = getting new users to the core action**. The NUX must lead to this action. Measuring MAUs or downloads without knowing if users are completing the core action is a vanity metric.

How to find your core action: do both bottom-up (analyze all possible actions, rank by "if user did X, what's their 7-day retention?") and top-down (if a user never does X, did they really use the product?). Pinterest found if you pinned something, 90%+ probability you returned the following week.

### Level 2: Retention — Product Gets Better With Use

Once users do the core action, the product must get **more valuable the more they use it** AND give users **more to lose by leaving**.

Pinterest's "Picked For You" feed was one of the first algorithmic feeds in a social product — the more you pinned, the more personalized your feed. You also accumulated boards (bookmarks for life goals, recipes, inspiration) — a mounting lock-in.

Evernote is the pure Level 2 product: infinite notes create a personal archive impossible to abandon. Its weakness: it has no Level 3.

Anonymity kills Level 2. Pure anonymity prevents accruing benefits and mounting loss. Pseudo-anonymity (persistent username) can still create lock-in. Products like Secret, Houseparty, and Clubhouse struggled to retain because (1) no accruing identity benefit and/or (2) engagement mechanics created overwhelming notification volume that inverted the network effect.

### Level 3: Self-Perpetuating Growth Loops

Every user interaction generates kinetic energy; the product's job is to **convert that energy back into growth or re-engagement**. Two types of loops:

- **Network effects**: each pin enriches Pinterest's graph, improving recommendations for all users — the strongest form
- **Growth loops**: supply-brings-demand (sellers invite buyers), or social re-engagement (Sarah pinned your pin → notification pulls dormant Lenny back)
- **Re-engagement loops**: notifications, collaborative experiences, social proof

Evernote has none of these — hence why they tapped out on growth and had to spend on acquisition.

TikTok is the rare exception: spent $1B+ on paid user acquisition *after* nailing Level 1 and Level 2, not before.

**Anonymity** also kills Level 3: no persistent identity means no accumulated social graph to leverage for re-engagement.

---

## Framework 2: The Hierarchy of Marketplaces

See also: [[hierarchy-of-marketplaces]]

Sarah's framework for building an enduring marketplace. Developed as a reaction against GMV-obsessed thinking, which leads founders to optimize for the wrong metric.

**Core insight**: Not all GMV is equal. $1M of GMV spread across 10 cities is worse than $1M in one city. The goal isn't GMV — it's **happy GMV**: a percentage of users retaining and returning after transactions.

### Level 1: Focus (the Thimble)

Focus ambition like a laser beam on a constrained market. Not a sun warming the ocean — a laser heating a thimble to boiling.

Why:
- Capital is scarce → must use it where it creates maximum flywheel velocity
- Founder attention is scarce → can't achieve minimum viable happiness at scale
- Competition is lower in narrow markets → easier to tip

Classic examples:
- DoorDash focused on suburbs (low competition, economically inefficient, but unchallenged) before expanding
- Postmates tried to do every city and every category simultaneously → spread too thin, unable to create happiness in any one segment
- Etsy: crafts at craft fairs → "earned secret" about fragmented handmade goods supply

**Minimum Viable Happiness**: the threshold at which a meaningful percentage of both sides of a transaction retain after the first transaction. Don't measure NPS — use Sean Ellis's "how disappointed would you be if this product disappeared?" If ≥40% say "very disappointed," you're on track.

### Level 2: Tip the Market

Once you've achieved minimum viable happiness in a constrained market, focus on reaching a **saturation point** that creates **tipping loops**:

1. **Growth loops** (supply-to-buyer, buyer-to-buyer, supply-to-supply):
   - REKKI: restaurant signs on → orders flow to supplier → supplier sees convenient order form → supplier sends REKKI their customer CSV → suppliers bring restaurants to REKKI
   - Hipcamp: buyer invites co-camper during checkout → viral loop
   - Uber/Lyft driver referrals → bloggers writing about earning referral bonuses

2. **Happiness loops** (churn the bad supply, reward the good):
   - Search ranking as a happiness loop: UberEats ranked fast-prep restaurants higher; Airbnb's review system churns poor hosts
   - Healthy churn on supply side is good in marketplaces (unlike consumer social) — you want to surface the best suppliers

Conditions for tipping a market:
- **Supply fragmentation** (concentrated supply won't lean in to your platform)
- **Low or no competition** (DoorDash in suburbs, Airbnb vs. HomeAway in budget stays)
- **High repeat use case** (not Thumbtack's plumber → forgotten by next use, have to start at Google)

### Level 3: Dominate the Market

Three simultaneous growth vectors once you have a playbook:
1. Penetrate your existing tipped market deeper (Uber: black car → UberX → UberPool)
2. Expand into adjacent markets/categories (carry your playbook to new geographies)
3. Blitz scale into as many new markets as capital and bandwidth allow — but always put more wood behind fewer arrows

Key rule: marketplace dominance is where the economics pay off. Graph of marketplace dominance vs. profitability is exponential — barely-number-one means fighting for each point of share; decisively dominant means near-zero customer acquisition cost.

Never rest: Grubhub dominated food delivery but failed to control its own delivery logistics, opening the door for DoorDash and Uber Eats. HomeAway/VRBO dominated vacation rental until Airbnb disrupted with a better experience.

### Finding Marketplace Opportunities

Three signal patterns:
1. **Take a low-NPS horizontal** → build a vertical (eBay → sneaker resale → GOAT/StockX)
2. **Bring a niche online** that's bigger than it looks (Hipcamp: casual camping land → eventual glamping; Etsy: craft fair goods)
3. **Change the atomic unit of supply** (Grubhub: restaurants with their own delivery → DoorDash/Uber Eats: any restaurant + third-party delivery)

LLMs may enable a 4th: automating the long tail of supply onboarding, making previously unscalable supply aggregation viable.

### Market Currents vs. Market Size

> "I think a lot of people think about markets like bodies of water — a big body of water we're going after. The most interesting markets you have to think of like currents. There's something creating a current that will pull a plank of wood forward."

Benchmark is deliberately contrarian on market size. They get excited by markets that appear small but have strong currents (forces of change creating momentum). Small markets with no competition let you tip the market faster. Markets that appear too small often have adjacent expansion potential.

## Actionable Advice
- Find your core action: if users never do X, they're not really users.
- Cohort by core action completion — not raw MAUs or downloads.
- Use "how disappointed would you be?" instead of NPS.
- Start with a thimble, not an ocean. Focus your ambition like a laser.
- Look for "earned secrets" — markets that haven't been addressed for structural reasons that have now changed.
- Marketplace builders: healthy supply-side churn is a feature, not a bug.

### Notable Quotes
> "Products should get better the more you use them, and users should have more to lose by leaving."

> "Think of markets like currents — there's something happening that's creating momentum that will pull a plank of wood forward."

> "GMV is to marketplaces what MAUs are to consumer social — a vanity metric. Focus on happy GMV."

> "Every strength has a corresponding weakness and vice versa." (attributed to Reid Hoffman)

## Sources
- [[sarah-tavel]] — "The hierarchy of engagement | Sarah Tavel (Benchmark, Greylock, Pinterest)"

## See Also
- [[hierarchy-of-engagement]] (framework)
- [[hierarchy-of-marketplaces]] (framework)
- [[two-sided-marketplace-dynamics]]
- [[network-effects]]
- [[product-market-fit]]
- [[retention]]
