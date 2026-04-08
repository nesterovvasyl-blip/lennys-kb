---
guest: Vijay Iyengar
episode: An inside look at Mixpanel's product journey | Vijay Iyengar
date: 2023-01-26
topics: [product-strategy, analytics, focus-vs-expansion, product-development, prioritization]
---

# Vijay Iyengar

## Background
Vijay Iyengar is Head of Product at Mixpanel, the product analytics platform. He transitioned from an engineering background — including stints as an engineer at Uber and as an engineering manager at Mixpanel — directly into a Director of Product role and then Head of Product, an unusual career path. He came from an engineering background similar to Lenny's own trajectory.

## Key Ideas
- **Invest profits, not people**: When expanding to new product lines, use profit or external capital — never pull engineers away from the core product. Diverting people from the core opens you to disruption by a competitor who out-invests you there.
- **Core focus recovery**: Mixpanel had ~40% revenue churn in 2018 because they spread engineering across product analytics, messaging, and data infrastructure. Cutting back to one product and prioritizing the top 10 churn reasons by ARR drove retention from 60% to 90% and NPS from 16 to 50 over ~3 years.
- **Design-led phase as a follow-on**: After the "build table stakes fast" phase, Mixpanel invested in system architecture and consistent UI (e.g., visualization consistency). This multiplied feature reach, since improvements applied everywhere rather than being rebuilt per product area.
- **Beware adjacent-category bolt-ons**: Secondary products that are #6 in their own category (CDP, feature flagging, messaging) contribute only 5–10% of revenue, don't accelerate growth, and steal engineering from the core. Category leadership in one area beats mediocrity in many.
- **RICE with a twist**: Standard RICE scoring prematurely deprioritizes high-reach/high-impact ideas because confidence and effort are murky for innovative bets. His fix: ignore C and E for a bit, explore the top ideas earnestly with engineers and designers, then re-add C and E once you have real signal.
- **Appetite over estimates**: Inspired by Basecamp's [[shape-up]] methodology, Vijay recommends picking a reasonable time box and then exploring "what would we do differently with 4 weeks vs. 8 weeks?" to find the efficient frontier of cost and impact.
- **Radical customer access for engineers**: Mixpanel pipes all customer feedback (NPS, support tickets, Twitter, win/loss notes) into Slack and Notion. Engineers can email customers directly; no PM gatekeeping. This builds a product mindset across the whole team.
- **Server-side tracking over client-side**: Client SDKs drop 20–30% of events on web (ad blockers, JavaScript issues) and create platform fragmentation on mobile. Server-side tracking is 100% cross-platform, instantly updatable, and feels natural for engineers who already log events.

## Frameworks & Mental Models
### Fix the Core Before Expanding
When facing 40% churn driven by feature gaps in the core: take the collected churn reasons, group by category, sort by ARR impact, and make the top 10 your roadmap. Give engineers direct access to the customers experiencing those problems. This is extreme but appropriate when the house is on fire.

### Product System Architecture
After closing table-stakes gaps, invest in the foundational "building blocks" of the product — the smallest set of primitives that can support many features. Notion's pages-and-blocks architecture is the reference example: every new feature inherits the entire design system automatically.

### Data Stack as Internal Tooling Multiplier
Using a reverse ETL tool (Census/Hightouch) to push enriched warehouse data (BigQuery) into Slack and Notion enables zero-code internal tools. Example: enriching every customer signal with ARR and CSM data makes engineers self-sufficient rather than bottlenecked by PMs.

## Memorable Quotes
> "If you're the leader in some core product, you should continue to out-invest everyone else in that core, and then invest the profits that come out of that core into the next venture. Invest profits and not people." — Vijay Iyengar

> "You can't mow your lawn while your house is on fire. You kind of put out the fire and then deal with everything else." — Vijay Iyengar

> "One of the things after you've been in engineering for a while is that you develop this tendency to immediately respond with 'no' to new ideas… The best way to get to a no, if you ultimately need to get there, is to try to make it work." — Vijay Iyengar

> "So many great products win or lose based on their architecture. Notion's pages-and-blocks architecture is so strong — you can hang so many features off those core building blocks." — Vijay Iyengar

## Actionable Advice
- When deciding whether to expand to a new product line, ask: will this take engineers away from the core? If yes, fund it from profits or VC, not people.
- If your product has high churn to competitors, list the top churn reasons by ARR and make them your roadmap before doing anything else.
- Give engineers direct access to raw customer feedback with no PM gatekeeper — pipe it into Slack unfiltered.
- Evaluate RICE scores, but first spend a week earnestly exploring high-reach/high-impact ideas before adding Confidence and Effort back in.
- Switch from client-side to server-side event tracking as your default. Supplement with client-side only for data that lives only in the browser.
- Use appetite-based time-boxing: pick a timeframe, then ask "what would we cut or change if we only had half the time?"

## Sources
- *An inside look at Mixpanel's product journey*, Lenny's Podcast, 2023-01-26

## Related Pages
- [[shape-up]]
- [[invest-profits-not-people]]
- [[product-system-architecture]]
