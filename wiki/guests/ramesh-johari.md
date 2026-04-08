---
guest: Ramesh Johari
role: Professor, Stanford University (data science and online marketplaces)
episode: "Marketplace lessons from Uber, Airbnb, Bumble, and more"
date: 2023-11-09
topics: [marketplaces, experimentation, data-science, pricing, growth, two-sided-platforms]
---

# Ramesh Johari

> Stanford professor who advises major marketplaces (Airbnb, Uber, Bumble, Stitch Fix, Upwork) on data science, experimentation, and the design and operation of two-sided platforms.

## Bio

Ramesh Johari is a professor at Stanford University focusing on data science methods, causal inference, and the design and operation of online markets. He was a research scientist and director of data science at oDesk (which became Upwork) from 2012, and has since advised Airbnb, Uber, Stripe, Bumble, Stitch Fix, and many others. His research sits at the intersection of statistics, economics, and marketplace design.

### What a Marketplace Actually Sells

Marketplaces don't sell rides or rooms — they sell the **removal of transaction costs** (friction). The host wants to earn money but can't find willing guests; the guest wants to stay somewhere but can't find willing hosts. The marketplace takes that friction away.

Implication: **both sides of the marketplace are customers.** Airbnb's customers include hosts, not just guests. Uber's customers include drivers. This is commonly misunderstood by founders and leads to systematically under-investing in supply-side experience.

### The Three-Part Data Science Flywheel

Ramesh's framework for how data science creates value in marketplaces:

1. **Finding matches** — Search, recommendations, ranking. Helping buyers find relevant sellers and vice versa.
2. **Making matches** — Triage, scoring applicants, helping users choose among options. Who should I interview? Which listing should I book?
3. **Learning from matches** — Rating systems, passive behavior signals, explicit reviews. What did we learn from this match to improve future ones?

These three form a cycle: what you learn from matches improves finding and making matches for the next round.

### The Prediction vs. Decision Distinction

Ramesh's most important principle: **prediction is about correlation; decisions require causation.** These are different problems and require different methods.

Classic mistake: send promotions to highest-LTV customers because the model predicts high LTV. But you don't care about their absolute LTV — you care about the *incremental LTV due to the promotion*. If high-LTV customers would have bought anyway, you've wasted the promotion and gotten the illusion of marketing effectiveness.

The right question is always: "What is the difference in outcome *because* I made this decision?" Not "what is the predicted outcome for this person?"

Practical implication: train your data scientists to think in terms of causal inference, not just predictive modeling. When they build an algorithm, ask: are we predicting what happened, or are we measuring the impact of a decision we're making?

### The Marketplace-Founder Myth

Ramesh argues we shouldn't have a concept of a "marketplace founder" — only founders. Every business has the option to become a platform as it scales (even OpenAI is now a marketplace via plugins). Thinking of yourself as a "marketplace founder" from day one creates failure modes:

1. **Premature marketplace thinking.** You can't build search-and-match algorithms when you have 10 users on each side.
2. **Overcommitting early.** Early monetization decisions (e.g., oDesk's perpetual % fee on all transactions) create social contracts with users that tie your hands later, enabling disintermediation.

The right question early: "What is my value proposition in a world where I don't have scaled liquidity on both sides?" This is always a specific, bespoke answer. For UrbanSitter, it was accepting credit cards. For oDesk, it was trust verification for remote workers.

**Scaled liquidity test:** Do you have a lot of buyers AND a lot of sellers? If yes, you're a marketplace. If only one side, you've won half the game — now decide whether to scale that side or attract the other. If neither, focus on a startup's fundamentals, not marketplace dynamics.

### A/B Testing Culture and Incentives

Ramesh identifies a systematic problem in companies that go "all-in on experimentation": the culture of winners and losers creates perverse incentives.

- Data scientists are judged on "wins" per quarter
- To get wins: run incremental tests (easier to detect small effects)
- To protect wins: run tests for too long (higher confidence in marginal improvements)
- Result: a constant treadmill of micro-optimizations, missing large opportunities

The better mental model: **learning is always a win.** Even a "failed" experiment that shifts your understanding of user behavior or product dynamics is a success. Bayesian A/B testing (incorporating prior learning into new experiments) provides a technical mechanism to reward this — when your prior shifts, you've contributed information that improves all future experiments.

The cultural norm change: in experiment launch docs, always specify what hypotheses are being tested about the business, not just what outcome you're hoping for. This makes "we learned X" a legitimate result even when the primary metric didn't move.

### The Cost of Learning

Every experiment has a cost — samples allocated to the control arm that could have been allocated to the better treatment. The "holdout" anecdote: a marketing manager secretly ran an unauthorized holdout all year, then told leadership at year-end: "That holdout cost you $2M — now you know what my team is worth." Brilliant, if unauthorized.

The lesson: **you have to pay to learn.** Companies that use "winner/loser" language are implicitly saying that testing a hypothesis that doesn't win was wasted time. This is wrong and destroys the culture of bold experimentation.

### Rating Systems: What Works and What Doesn't

On designing marketplace review systems:

- **Rating inflation** is universal — over time, median ratings drift upward due to social reciprocity and norming (a 4-star feels like an insult when everyone else gets 5).
- **Renorming the scale:** rather than 1–5 stars, use language like "exceeded expectations" for top rating. Even better: ask users to compare to a previous experience they rated highly.
- **Distributional fairness:** simple averaging harms new entrants disproportionately. An early negative review can cause an 8% revenue hit and predict platform exit (per oDesk/eBay research). Consider pulling new entrants toward a prior (e.g., community average) until they accumulate reviews.
- **Airbnb's double-blind reviews** (Lenny led this): holding reviews until both parties submit increases review rate significantly (social pressure to respond), giving more data. Information is also contained in *non-reviews* — platforms like eBay found that "effective percent positive" (normalizing by including non-reviews in the denominator) better predicted downstream seller performance.

## Actionable Advice

- Define your value proposition for the pre-liquidity state before worrying about marketplace design
- Train your data team to think about causal inference, not just predictive accuracy
- Measure "what decision are we making, and what's the incremental impact of this decision?" not just "what will happen?"
- Build experiment launch docs around hypotheses, not just hoped-for outcomes
- Change the language from "wins and losses" to "what did we learn?" — especially for bold experiments
- Design rating systems with distributional fairness in mind — protect new entrants with priors
- Recognize marketplace whac-a-mole: most changes create winners and losers, not net new value; focus on whether the winners matter more to your business

## Notable Quotes

> "What they're taking away is the friction of finding a place to stay. They're taking away the friction of finding a driver. Marketplaces are selling you the taking away of something."

> "Predicting is about picking up patterns, but making decisions is about thinking about differences. That's the distinction between causation and correlation."

> "It's almost never about building a marketplace when you're building a marketplace."

> "Experimentation was never historically in science about winners and losers. Experimentation is hypothesis-driven. It's about what are you learning?"

> "Marketplaces are a little bit like a game of whac-a-mole. Many of the changes that are most consequential create winners and losers."

## Sources

- [[ramesh-johari]] — "Marketplace lessons from Uber, Airbnb, Bumble, and more"

## See Also

- [[network-effects]]
- [[experimentation-culture]]
- [[long-term-holdout-experiments]]
- [[two-sided-marketplace-dynamics]]
- [[product-led-growth]]
