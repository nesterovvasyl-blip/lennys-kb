---
guest: Ramesh Johari
role: Professor, Stanford University (data science, online markets and platforms)
episode: "Marketplace lessons from Uber, Airbnb, Bumble, and more | Ramesh Johari (Stanford professor)"
date: 2023-11-09
topics: [marketplaces, data-science, experimentation, rating-systems, growth]
---

# Ramesh Johari

> Stanford professor and marketplace data science authority who argues that marketplaces are really "friction removal" businesses — and that every founder is already a marketplace founder.

## Bio

Ramesh Johari is a professor at Stanford University specializing in data science methods and the design and operation of online markets and platforms. Beyond academia, he has directed data science at oDesk (now Upwork), and advised or collaborated with Airbnb, Uber, Stripe, Bumble, Stitch Fix, and Upwork. He brings rigorous academic thinking about causality and incentive design to real marketplace challenges.

## Key Ideas

### What Marketplaces Actually Sell: Friction Removal

Customers think Airbnb sells rooms and Uber sells rides. In reality, both sell the *removal of transaction costs*. Hosts and drivers are selling to customers; Airbnb and Uber are selling to both sides by eliminating the friction that would otherwise prevent transactions from happening. This framing has critical implications:

**Both sides are customers**: Hosts need Airbnb as much as guests do. Drivers need Uber as much as riders do. Both sides depend on the platform to do its core job (remove friction); alienating either side breaks the business.

**Disintermediation is the enemy**: When a freelancer hands a client their business card after an Upwork job, the platform loses. Long-term relationships on oDesk had this problem: after trust was established, the platform's value (verifying work, ensuring payment) was marginal but it still took 10% of transactions.

### Every Founder Is a Marketplace Founder

Ramesh argues that virtually every business that can be disrupted by online transactions will eventually face the choice of becoming a platform. OpenAI is now a marketplace (plugins create a two-sided dynamic). Substack started as a newsletter tool and evolved into a demand-generation marketplace for writers.

The corollary: stop thinking about yourself as a "marketplace founder" if you don't yet have scaled liquidity on both sides. Focus on solving one pressing friction first.

> "A marketplace business never starts as a marketplace business, because what we think of as a marketplace business is something which at scale is removing the friction of the two sides finding each other. But when you start, you don't have that scale."

### The Liquidity Litmus Test

Ramesh's test for whether you're actually a marketplace: "Do you have scaled liquidity on both sides?" If not — regardless of what you call yourself — you're not yet a marketplace. Implications:

- If you have one scaled side, use it to attract the other (Uber subsidized drivers in new cities with promotions, then used the driver pool to attract riders)
- If you have neither, focus on being a startup first: solve one pressing pain point without needing the marketplace scale to do so

Example: UrbanSitter started by solving babysitter payment (allowing credit cards instead of requiring cash), not by solving "the marketplace matching problem." That initial friction-removal generated enough liquidity to then build the marketplace.

### The Data Science Flywheel: Find, Make, Learn

Marketplace data science has three interconnected functions that compound:

1. **Finding matches**: Search, recommendations, ranking algorithms
2. **Making matches**: Triaging applicants, surfacing relevant options
3. **Learning from matches**: Ratings, reviews, passive behavioral signals

These form a cycle: better learning makes better finding which enables better making, and so on. All three require data science, and all three are fundamentally about taking friction away through information.

### Causation vs. Correlation: The Critical Data Science Distinction

The most important thing any data scientist can do is understand the difference between predicting outcomes (correlation) and making decisions (causation). Example: sending high-LTV promotions to your highest-LTV customers seems logical — but high LTV is predicted from past patterns, not caused by your promotion. The right question is: "What is the *marginal* increase in LTV from sending the promotion to this person?"

This matters because prediction algorithms trained on past data perpetuate past patterns. A hiring algorithm that predicts who will be hired just learns to surface candidates who look like past hires — it doesn't tell you which candidates will *add more value* than the others.

> "Prediction is inherently about correlation. But when we ask people to make decisions, we're asking them to think about causation."

### Experiments: Culture, Incentives, and the "Fat Tails" Problem

Ramesh is a strong believer in experimentation but identifies key failure modes in experiment-heavy cultures:

**The incentive trap**: When data scientists are evaluated on "wins," they run incremental experiments (more likely to win) and run them too long (to ensure statistical significance). This kills exploration of high-variance ideas.

**Fat tails matter**: A Microsoft research paper shows that experiment cultures should accept larger, riskier experiments — even if they fail more often. A "failed" experiment that teaches something meaningful about your business is a success.

**The cultural fix**: Replace the language of "winners and losers" with "learning." Experiments that generate valid negative results are valuable because they move the *prior* for all future experiments. Bayesian A/B testing operationalizes this — it allows past learning to be encoded into the analysis of current experiments.

**Learning has a cost**: Holding out a control group costs revenue in the short term (real example: a marketing team's unauthorized holdout that cost millions). This cost is justified because without it, you can't know what your program was actually worth.

### Rating Systems: Inflation, Averaging, and Distributional Fairness

Rating systems are understudied and poorly designed across most marketplaces. Key issues:

**Rating inflation**: Over time, median ratings on platforms like Uber and Upwork creep upward. Causes: social reciprocity (people don't want to leave bad reviews for someone they've met), norming (4 stars eventually feels mean). Fix: use relative comparisons rather than absolute scales ("Did this exceed your expectations?" or "How does this compare to your best stay?").

**The averaging problem**: Platforms that average all ratings give overwhelming advantage to established sellers (10,000 reviews: one bad review is invisible) at the expense of newcomers (first bad review has an outsized negative impact). Early research on eBay found a first negative rating caused an 8% immediate hit to revenue and predicted exit from the platform.

**Distributional fairness**: One solution — use Bayesian priors rather than simple averages. New sellers start with a prior based on marketplace norms; ratings update that prior. This prevents one bad early review from permanently disadvantaging a new participant.

## Key Quotes

> "Marketplaces are a little bit like a game of whac-a-mole... Many of the changes that are most consequential create winners and losers." — Ramesh Johari

> "It's almost never about building a marketplace when you're building a marketplace." — Ramesh Johari

> "What AI has done for us is it's massively expanded the frontier of things we could think about our problem. And I really think what that does is puts more pressure on the human, not less." — Ramesh Johari

> "Slow down. We're so convinced that speed is the way you're going to find the right answer, that we don't slow down to develop meaningful mental models." — Ramesh Johari

## Actionable Advice

- Before calling yourself a "marketplace founder," apply the liquidity litmus test: scaled liquidity on both sides?
- Identify the one pressing friction customers face *before* you have marketplace scale, and solve that first
- Train your data science team to ask "what decision does this analysis support?" not just "what does this predict?"
- When running experiments, embrace "fat tails" — allow higher-variance tests that may fail but generate meaningful learning
- Design rating systems to correct for inflation by using relative comparison prompts
- For new marketplace sellers, use Bayesian priors rather than raw averages to protect against early negative review asymmetry
- Tell your data scientists to look at actual examples of your data, not just statistical summaries (the "shoe leather" approach)

## Related Pages

- [[concepts/marketplaces]]
- [[concepts/experimentation-culture]]
- [[concepts/network-effects]]
- [[frameworks/marketplace-data-science-flywheel]]
