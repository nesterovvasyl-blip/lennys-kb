---
guest: Ronny Kohavi
role: Consultant and Instructor; former VP Technical Fellow at Airbnb, Technical Fellow at Microsoft, Director at Amazon
episode: "The ultimate guide to A/B testing | Ronny Kohavi (Airbnb, Microsoft, Amazon)"
date: 2023-07-27
topics: [experimentation, ab-testing, metrics, data-driven, growth, product-development]
---

# Ronny Kohavi

> Ronny Kohavi is the world's leading expert on A/B testing and experimentation, author of Trustworthy Online Controlled Experiments, and has run experimentation platforms at Amazon, Microsoft, and Airbnb.

## Content

Ronny Kohavi spent his career at three of the world's most data-driven companies: Amazon (Director of Data Mining and Personalization), Microsoft (Corporate VP leading the Microsoft Experimentation Platform — ExP), and Airbnb (VP and Technical Fellow). He is the author of *Trustworthy Online Controlled Experiments* (all proceeds donated to charity), translated into Chinese, Korean, Japanese, and Russian. He now consults, teaches, and runs a cohort course on Maven.

### The Most Surprising Experiment Result in History

Ronny's opening example: at Bing, someone proposed moving the second line of ad text to the first line, making the title larger. It had languished in the backlog for months — people rated it as uninteresting. An engineer spent a couple of days implementing it and launched it. Revenue alarms fired. Everyone assumed a bug. After extensive verification — no bug. This single change was **worth $100 million to Bing at the time**, the largest revenue impact in its history. The user experience metrics were not significantly harmed.

The lesson: "We are often humbled by how bad we are at predicting the outcome of experiments."

### The Real Failure Rate of Experiments

Ronny has published three different failure rates from his career:
- **Microsoft overall**: ~66% of ideas fail
- **Bing specifically**: ~85% failure rate (harder to improve an already-optimized product)
- **Airbnb search**: **92% failure rate** (only 8% of experiments improved the key metric)

Industry benchmarks from Google Ads, Booking.com, and others: 80–90% failure rates are typical.

This humbling reality is universal. Every new team that starts running experiments believes they will have a higher success rate than the industry. They are all wrong. The reason this matters: if you don't know that 66–92% of your ideas are failing, you are shipping a lot of things that are flat or negative without realizing it.

### The OEC: Overall Evaluation Criterion

The most common mistake in A/B testing is optimizing for the wrong thing. "Improve revenue" is an incomplete OEC because you can always increase revenue in the short term by hurting user experience (e.g., displaying more ads). A good OEC must:

1. Be **causally predictive of lifetime value** — not just short-term metrics
2. Include **countervailing guardrail metrics** — so you know if you're buying short-term wins at the cost of long-term retention

At Bing: they modeled the relationship between ad density and user session quality, then framed ad optimization as a *constraint satisfaction problem* — maximize revenue per pixel of vertical ad space. This prevented the "add more ads" local maxima.

At Amazon's email team: when recommendations were measured purely by clicks-from-email, the team scaled spam to maximize the metric. Fix: model the cost of unsubscribes as a dollar value, subtract from revenue. Result: more than half of active campaigns were actually net-negative once unsubscribe costs were included.

At Airbnb: a good OEC for booking conversion includes not just whether someone booked, but whether they *liked the stay* — measurable months later. This requires building predictive models from historical data.

### When to Start Running Experiments

The rule of thumb: you need **at least 200,000 users** to reliably detect 5%+ improvements. Below tens of thousands of users, statistics don't work for most product metrics. Startups should:
- Below 200K: Start building the platform and culture. Run tests when you can but focus on large-effect experiments (5–10% improvements).
- Above 200K: The magic begins. Test everything. Move toward zero marginal cost per experiment.

### Twyman's Law: If It Looks Too Good, It's Probably Wrong

Twyman's Law (originally coined in UK radio/media): any figure that looks interesting or unusual is usually wrong.

Ronny's application: if your typical experiment moves a metric 0.5–1% and you see a 10% movement, hold the celebration. In 9 out of 10 cases when he has invoked Twyman's Law, they found a flaw. The $100M Bing result was the exception, and it was replicated multiple times before acceptance.

### Sample Ratio Mismatch: The Most Common Experiment Error

If your experiment is designed 50/50 control/treatment and you get 50.2/49.8 — that might sound close but could be a red flag. For a million-user experiment, the probability of getting 50.2/49.8 by chance can be one in half a million. Something is wrong.

At Microsoft, ~8% of experiments suffered from sample ratio mismatches. Common causes:
- Bots (treatment changes a webpage, bots fail to parse it and retry disproportionately)
- Data pipeline issues
- Marketing campaigns that skew assignment distribution
- Incorrect randomization logic

Ronny's team responded by **blanking out experiment scorecards** when sample ratio mismatch was detected, forcing engineers to acknowledge the problem before seeing results — because warning banners were simply ignored.

### P-Values: The Common Misinterpretation

Most practitioners believe: P-value of 0.02 means 98% probability the treatment is better. **This is wrong.**

P-values are *conditional probabilities* — they assume the null hypothesis is true and calculate the probability of seeing data this extreme by chance. To get the actual probability you want (probability treatment is truly better), you need Bayes' Rule, which requires knowing the prior probability of success.

Practical implication: at Airbnb search where only 8% of experiments succeed, a statistically significant result (P < 0.05) has a **26% false positive rate** — not 5%. The solution: require P < 0.01 for borderline results, and replicate results using Fisher's or Stouffer's combined test.

### Building an Experimentation Platform

Key principles:
- **Goal**: reduce marginal cost of running an experiment to near zero
- At Microsoft/Bing: 20–25,000 experiments per year, ~100 new treatments per working day
- Platforms should auto-generate scorecards so data scientists aren't bottlenecks
- Build/buy is not zero-one: third-party tools today are much better than they were in Amazon's era
- The best place to start: find a team that launches frequently (weekly/daily, not yearly) and has a clear OEC

For culture change: find a beach-head team. Share surprising results broadly. Cross-pollination of people trained in experimentation is the most reliable way to spread the culture.

### Big Redesigns Almost Always Fail

Ronny has documented numerous large product redesigns that significantly hurt key metrics. The right approach: incrementalize. Instead of shipping 17 changes at once (where most will fail), ship one factor at a time (OFAT: one factor at a time), learn, adjust. Of 17 changes, maybe 4 are genuinely good — ship those.

Sunk cost fallacy trap: "We already spent six months building this." A data-driven organization will not launch something that's negative for users regardless of investment. Don't.

### Actionable Advice
- Define your OEC to be causally predictive of lifetime value, with countervailing guardrail metrics
- Expect 66–92% of your experiments to fail — this is not a sign of bad teams, it's the universal reality
- Always run sample ratio mismatch checks on your experiments
- Treat statistically significant results with skepticism proportional to their magnitude (Twyman's Law)
- Use Bayesian priors (historical success rate) to estimate true false positive rates
- Do quarterly reviews of your most surprising experiments — build institutional memory
- Replicate borderline results rather than shipping on P < 0.05 alone

### Notable Quotes
> "I'm very clear that I'm a big fan of test everything — any code change that you make, any feature that you introduce has to be in some experiment."

> "We are often humbled by how bad we are at predicting the outcome of experiments."

> "If you go for something big, try it out, but be ready to fail 80% of the time."

> "If something is not statistically significant, that's a no-ship, because you've just introduced more code and increased maintenance overhead."

> "If you think you've got a 5% type one error rate, using real-time P-value monitoring to stop experiments early, you'd probably have a 30% error rate."

## Sources
- [[ronny-kohavi]] — "The ultimate guide to A/B testing | Ronny Kohavi (Airbnb, Microsoft, Amazon)"

## See Also
- [[experimentation-culture]]
- [[ab-testing-principles]]
- [[long-term-holdout-experiments]]
- [[overall-evaluation-criterion]]
