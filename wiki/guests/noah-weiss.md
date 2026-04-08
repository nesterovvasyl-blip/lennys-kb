---
guest: Noah Weiss
role: Chief Product Officer, Slack (2016-present); former Head of Product, Foursquare; former PM, Google and Fog Creek Software
episode: "The 10 traits of great PMs, AI, and Slack's approach to product | Noah Weiss (Slack, Google)"
date: 2023-07-23
topics: [product-management, slack, ai, team-building, product-led-growth, pm-traits, consumer-to-b2b, product-principles]
---

# Noah Weiss

> The CPO of Slack who codified the 10 traits of great product managers and built the practices that make Slack one of the most beloved enterprise products.

## Bio

Noah Weiss is Chief Product Officer at Slack, where he has spent seven years leading all aspects of product including self-service, huddles, clips, and AI. Before Slack, he was Head of Product at Foursquare (2010-2015), where he has extensive scar tissue from the consumer social product's rise and fall. Prior to that, he was a PM at Google (working on what became the knowledge graph) and Fog Creek Software. A new father who did a full digital detox on paternity leave, he's deeply thoughtful about the craft of product management and its evolution.

## Key Ideas

### The 10 Traits of Great Product Managers

Noah wrote a widely-shared post on this topic as an alternative to the "PM as mini-CEO" framing, which he calls "the most dangerous piece of advice ever in the history of product management" because it produces dictatorial PMs who get rejected by their teams.

The 10 traits (not in strict priority order):

1. **Live in the future and work backwards**: Carve out time for 6-month to 2-year horizon thinking; immerse in the problem space and bring inspiration back to the team

2. **Amplify your team**: Facilitate ideas, create energy and momentum; the PM is a multiplier of others' output, not a creator of their own

3. **Impeccable execution**: Be organized, follow through, set clear expectations. Creates the "I've got this" aura that earns trust and more responsibility. Ben Horowitz formulation: say what you're going to do, do what you said, and explain why if you can't

4. **Focus on impact**: For customers first, then the business. "Impact solves all PM issues" — consistently shipping things people love overrides everything else

5. **Facilitate the pace and quality of decision-making**: Not making all the decisions, but creating the conditions for the team to make high-quality decisions quickly; this is the actual job, not being the tiebreaker

6. **Optimizing for learning**: Especially at senior levels, willingness to sacrifice near-term impact for the sake of discovering new levers; portfolio approach to product bets

7. **Write well**: The only scalable way to influence a large product org; recommended: *On Writing* by Stephen King, *Creative Selection* about Apple's iterative product development

8. **Data fluency**: Not necessarily statistics, but enough fluency in quantitative data, surveys, and customer interviews to make higher-likelihood product bets

9. **Product taste**: Intuition for what customers will love before you're able to test it; develops through immersion in customer problems and creative work

10. **Living in the future and long-horizon thinking**: (see #1; revisited specifically for senior PMs as strategy ownership)

For early-career PMs: focus on execution, impact (even local impact), and data/research fluency.
For senior PMs: focus on facilitating decision quality, long-horizon strategy, and writing.

### Complaint-Storms: Structured Empathy Building

Noah's process for developing fresh eyes on your own software, especially when the team has become too expert to see friction.

How it works:
1. Assemble team including Stewart Butterfield (Slack's CEO) or equivalent founder/exec
2. Start with a **competitor or adjacent product** first — walk through the customer journey from website through account creation to first value
3. Everyone fills in every friction point, confusion, and pain point they observe as they go, projected on one screen
4. After building the muscle on someone else's product, run the same process on your own product

Benefits:
- Competitor first removes defensiveness ("everyone has issues — it's not just us")
- Calibrates the team on product quality standards
- Generates a prioritized burndown list for "customer love" work
- Surfaces systemic issues that don't show up in any individual metric

Related: Slack has a **Customer Love Sprint** — a two-week hackathon where teams sprint on the lowest-effort/highest-impact changes from the complaint-storm list. Goal: ship all of them. Quarterly cadence for user-facing teams, twice-yearly for others.

### Slack's Self-Service Plateau and Turnaround (2019)

Around 2019, Slack's self-service business metrics stopped being as healthy as they'd been in the 2014-2017 hypergrowth era. Root cause: the product had excellent product-market fit with technologically sophisticated early adopters, but the next wave of customers had fundamentally different needs.

The turnaround approach:
1. **Throw out the existing roadmap** rather than optimizing what already existed
2. **Six-month learning sprint**: commit to no impact, only learning about new levers
3. **Key insight on comprehension/desirability**: New users didn't comprehend what Slack was for or why they should care — not a product problem, but a framing and experience problem
4. **Trial strategy**: Slack had never let users taste the paid product — they went from free tier directly to paid. Implementing a trial of premium features was one of the biggest levers
5. **New north star metric — "Successful Teams"**: Research showed teams with 5+ people communicating in Slack the majority of the work week were 400% more likely to upgrade in 6 months. This low bar (not even daily usage!) became the shared goal across all product teams, shifting focus from top-of-funnel to early activation

Result: doubled the rate of new paid customer growth over the following 1-2 years.

### Working with Product-Minded Founders

Noah has worked with both Dennis Crowley (Foursquare) and Stewart Butterfield (Slack) — both strongly opinionated founders in the PM's domain. Key lessons:

**U-curve model of founder involvement**:
- High involvement at the **start** (strategic buy-in, agreed principles, anti-goals)
- Lower involvement during **team execution and exploration**
- High involvement again at the **end** (quality bar, taste test the soup)

The failure mode: not doing the final step, which means the founder sees the product for the first time at launch and is unhappy. Solution: founder joins the team in a live bug bash — everyone looking at real software together trying to raise the quality bar, not the founder reviewing static mocks saying "no."

**Establishing shared principles**:
Convert founder taste into a shared language. Slack's four product principles (largely stable for 4-5 years):
1. **Be a great host** — relentlessly save people's steps; anticipatory design
2. **Don't make me think** — design for people from diverse backgrounds who shouldn't need to customize much
3. **Take bigger boulder bets** — actively resist incrementalism; the mental metaphor is "get to the next hill" to see the mountain range beyond
4. **Customer-obsessed, competitor-aware** — obsess over customers, stay aware of but not paralyzed by competitors

### AI in Products: 15 Years of Principles

Noah worked on what became Google's Knowledge Graph, ran recommendation systems at Foursquare, and has been prototyping LLM-based products at Slack.

Hard-won principles:
- **The UI promise must match the quality of the underlying model**: LLMs appearing supremely confident while hallucinating is a trust-destroying mismatch. Be transparent about uncertainty
- **Design for virtuous training cycles**: Product experiences should generate training data as a byproduct (Netflix ratings → better recommendations model)
- **Parallel incubation**: When a new capability emerges (AI), create a few small parallel teams using shared ML infrastructure but exploring different customer problems, rather than forcing all existing teams to add AI to their roadmaps immediately. Steady state = AI becomes part of every team's roadmap just as mobile is today

### Foursquare's Lessons: Framing and Competitive Timing

The Foursquare decline offers a clear lesson on atomic unit framing. The company bet that the atomic unit of social sharing would be "a person at a place." Instagram (early Foursquare API user) discovered it was "a person having a moment" — sometimes with a place, often without. That single framing difference redirected all the social behavior to Instagram. Compounded by Google Maps eventually replicating local discovery on a 1B+ user distribution platform.

The B2B pivot lesson: "The feedback you get from people willing to pay for your product is so much faster than can I build a large-scale consumer business and when they hope to have enough reach to slap ads onto it."

## Key Quotes

> "Mini-CEO is the most dangerous piece of advice ever in the history of product management." — Noah Weiss

> "Impact solves all PM issues — if a team is consistently building things people love and changing the direction of the business, everything else is just an input." — Noah Weiss

> "Product market fit is almost like you keep stacking these S-curves — you get PMF in a small group, then exponential growth, then you hit the ceiling and have to jump to the next S-curve." — Noah Weiss

> "We're customer-obsessed, competitor-aware. We obsess about customers. We build something they'll love enough to tell their coworkers and the rest takes care of itself." — Noah Weiss

> "Taking bigger boulder bets. Get to the next hill to see what the horizon looks like around you." — Noah Weiss

## Actionable Advice

- Replace "PM as mini-CEO" with "PM as decision-quality facilitator" — the team should make better decisions, with or without your input
- Run complaint-storms on competitor products before running them on your own; calibrate team on quality standards first
- When a growth metric plateaus, consider a 6-month learning sprint rather than optimization of existing bets
- Define your activation metric as the early behavior that predicts long-term retention/revenue (Slack: 5 people communicating the majority of the workweek = 400% upgrade likelihood)
- Get founders involved at the beginning of projects (strategy/anti-goals) and at the end (taste test in real software) — not throughout
- For AI: design for uncertainty transparency and virtuous training cycles from day one
- Create a pilot customer program with diverse industries/sizes and pain-tolerant champions to test features before broad launch

## Related Pages

- [[concepts/product-led-growth]]
- [[concepts/product-market-fit]]
- [[frameworks/radical-candor]]
- [[frameworks/shape-up]]
- [[concepts/experimentation-culture]]
