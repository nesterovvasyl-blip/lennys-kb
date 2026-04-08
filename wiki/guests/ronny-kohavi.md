---
guest: Ronny Kohavi
role: Consultant, Teacher, Author; former VP & Technical Fellow at Airbnb, Technical Fellow at Microsoft, Director at Amazon
episode: "The ultimate guide to A/B testing | Ronny Kohavi (Airbnb, Microsoft, Amazon)"
date: 2023-07-27
topics: [a-b-testing, experimentation, data-driven-culture, metrics, oec, trustworthy-experiments, statistics, product-development]
---

# Ronny Kohavi

> The world's foremost authority on A/B testing and online controlled experiments, who built experimentation platforms at Amazon, Microsoft (Bing), and Airbnb and authored the definitive book on the subject.

## Bio

Ronny Kohavi, PhD, is a consultant and instructor who is widely considered the world expert on A/B testing. He was VP and Technical Fellow at Airbnb, Corporate VP at Microsoft (where he built the Microsoft Experimentation Platform and ran Bing experimentation), and Director of Data Mining and Personalization at Amazon. He is the author of *Trustworthy Online Controlled Experiments: A Practical Guide to A/B Testing* (all proceeds donated to charity) and teaches a live cohort-based course on Maven.

## Key Ideas

### Most Ideas Fail — Embrace It

The single most important fact about experimentation: the majority of ideas fail. Across Ronny's career:
- **Microsoft overall**: ~66% of ideas fail (two thirds)
- **Bing** (highly optimized domain): ~85% failure rate
- **Airbnb search relevance**: ~92% failure rate

These numbers are consistent with external benchmarks — Booking.com, Google Ads, and others report 80-90% failure rates. The implication: if you're not running experiments, you're likely shipping 70%+ of your features that are either neutral or harmful.

"Flat to me, if something is not statistically significant, that's a no-ship, because you've just introduced more code. Maintenance costs will go up."

### Surprise as the Signal for Learning

Ronny defines "surprising" in a specific, useful way: an experiment is surprising when **the predicted outcome and actual outcome differ significantly**. Not just when the result is positive. Surprising losses (expected to win, massively negative) teach as much as surprising wins. The quarterly "most interesting experiments" meeting — not the most successful, but the most surprising — is one of the highest-leverage institutional learning rituals he recommends.

The canonical example: a Bing engineer spent two days implementing a tiny change (promoting the second ad title line to the first position). Everyone ignored it in the backlog for months — it seemed like a "meh" idea. It generated $100 million in incremental revenue, the biggest single revenue improvement in Bing's history. Nobody predicted it.

### The OEC: Overall Evaluation Criterion

The most common mistake in A/B testing is optimizing for the wrong metric. Revenue is the obvious target, but you can always increase short-term revenue by degrading user experience (more ads, darker patterns). The OEC is the composite metric designed to be **causally predictive of long-term user lifetime value**.

A good OEC:
- Balances revenue metrics with guardrail user experience metrics
- Prevents short-term optimization that destroys long-term value
- Should be directionally agreed-upon by the whole team before testing begins

The Amazon email team case study: they initially measured "revenue from email-attributed clicks." More emails = more revenue credit. This led to spam. The fix: add the cost of unsubscribes (modeled at a few dollars each). More than half their email campaigns became negative once the unsubscribe cost was included. The OEC revealed the right behavior.

The search ads OEC at Bing: number of ads is not free — Ronny's team ran experiments to map exactly how each additional ad reduced session success rate and increased churn, then set a "pixel budget" — a constraint that forced the ad team to achieve the same revenue within the same space, forcing actual quality improvement.

### Trust Is the Foundation of Experimentation

The most commonly cited goal of experimentation is "speed." Ronny argues the actual bottleneck is trust. If your experimentation platform produces untrustworthy results, the organization will stop using it, cherry-pick results, or launch bad products with false confidence.

The Optimizely case: early Optimizely used real-time P-value monitoring (stopping an experiment when the P-value crossed 0.05). This inflates the false positive rate from 5% to ~30%. Companies were seeing "wins" they couldn't replicate — and eventually lost trust in experimentation. Optimizely fixed it after researchers pointed this out.

Ronny's trust-building practices:
- **Sample ratio mismatch (SRM) detection**: if your 50/50 split produces 50.2/49.8, that's a red flag. At Microsoft, ~8% of experiments had SRM — caused by bots, data pipeline issues, or incorrect assignment. Blank out the scorecard when SRM is detected.
- **A/A testing**: run an experiment where both variants are identical; any "significant" result is a false positive and reveals platform bugs.
- **Replication**: for results at 0.01 < p < 0.05, run again and combine results using Fisher's or Stouffer's method.

### P-Values: The Common Misinterpretation

Most practitioners read a p-value of 0.02 as "98% probability the treatment is better than control." **This is wrong.** A P-value is the probability of seeing this data *assuming the null hypothesis is true* — not the probability that the treatment is better.

To get the probability most people actually want (is the treatment better?), you need Bayes' rule and a prior on your success rate. At Airbnb, with an 8% experiment success rate, a statistically significant result at p < 0.05 has a **26% false positive rate** — not 5%. This is why Ronny required replication for borderline results.

### When to Start A/B Testing

Practical threshold: you need at least **tens of thousands of users** for statistics to work on most metrics. For a retail site trying to detect 5%+ improvements in conversion rate, you need around **200,000 users**. Below that, start building the culture and platform infrastructure so you're ready when you scale.

"Start below 200,000 users, but start building the culture, platform, and integration so that as you scale, you start to see the value."

### Experimentation Shouldn't Block Big Bets

A common objection: "experimentation leads to local maxima and prevents innovation." Ronny's response: the solution is a portfolio approach, not abandoning experimentation.
- ~70-80% of experiments: incremental improvements in known directions
- ~20-30%: high-risk, high-reward bets designed to break out of local maxima

For big redesigns: decompose the redesign into the smallest possible independent factors (OFAT — one factor at a time). Test incrementally toward the new design. Even if you do a full redesign, run it as a test — "be ready to fail 80% of the time." The sunk cost fallacy is real: teams invest months in a redesign, it tests negative, and they ship it anyway.

### Institutional Memory

The value of experiments isn't just in individual decisions — it's in accumulated organizational knowledge. Ronny's practices:
- Maintain a searchable database of all past experiments with keywords
- Run quarterly "most interesting experiments" reviews to surface surprises
- Document what was expected vs. what happened (surprise = valuable learning)

Without institutional memory, hard-won lessons get forgotten as people leave. Ronny re-introduced the "open link in new tab" pattern at Airbnb after discovering it had been a significant win at Microsoft 10+ years earlier but had been forgotten.

## Frameworks

### Hierarchy of Evidence

When evaluating any claim or research finding, trust is proportional to the quality of the evidence:
1. Anecdotal (lowest trust)
2. Observational study
3. Natural experiment
4. Controlled experiment
5. Multiple replicated controlled experiments (highest trust)

## Key Quotes

> "I'm very clear that I'm a big fan of test everything — any code change you make, any feature you introduce has to be in some experiment." — Ronny Kohavi

> "We are often humbled by how bad we are at predicting the outcome of experiments." — Ronny Kohavi

> "When the result looks too good to be true — hold the celebratory dinner, investigate." (Twyman's Law) — Ronny Kohavi

> "If you go for something big, try it out, but be ready to fail 80% of the time." — Ronny Kohavi

> "If in peace time you're wrong two thirds to 80% of the time, why would you be subtly right in wartime?" — Ronny Kohavi (on COVID decision-making)

## Actionable Advice

- **Define your OEC before running your first experiment** — if your team can't agree on whether "more time on site" is good or bad, your OEC is broken.
- **Build SRM detection into your platform from day one** — 8% of experiments at Microsoft were invalid due to sample ratio mismatches; catching this early prevents false decisions.
- **Don't ship on flat** — neutral results mean code added without benefit. Don't do it unless legally required.
- **Start with a beachhead team** — find one team that ships frequently, build the culture and platform there, then let success and cross-pollination spread it.
- **Document surprises quarterly** — organize a "most interesting experiments" meeting, not just "most successful experiments."
- **Replicate borderline results** — for p-values between 0.01 and 0.05, run the experiment again and combine results before declaring a winner.

## Related Pages

- [[concepts/experimentation-culture]]
- [[frameworks/long-term-holdout-experiments]]
- [[concepts/data-flywheel]]
- [[frameworks/okrs-radical-focus]]
