---
aliases: []
guests: [albert-cheng, adam-fishman, jackson-shuttleworth, itamar-gilad, ronny-kohavi]
---

# Experimentation Culture

> Building organizational habits around continuous A/B testing, where the volume of experiments is itself a strategic forcing function.

## Content

Experimentation culture goes beyond having A/B testing infrastructure — it means making continuous experimentation a core organizational habit, embedded in how teams plan, build, and learn.

**Key elements:**

- **Growth model**: A documented theory of how the product grows, which defines what to test and why
- **Instrumentation**: Event tracking and data pipelines that make experiment analysis fast and trustworthy
- **No-code testing tools**: Empowers non-engineers (PMs, marketers, designers) to run experiments without eng bottlenecks
- **Cross-functional experimentation**: Tests that span product, growth, marketing, and monetization rather than siloed within one team
- **Broad socialization of learnings**: Experiment results shared widely so the whole org builds intuition about what works

**Albert Cheng's "1,000 experiments/year" target at Chess.com** is a notable case study. The specific number is less important than its function: it's a forcing function that compels the organization to invest in tooling, reduce experiment cycle time, and train people at all levels to think experimentally. When you commit to 1,000 experiments, you quickly discover every bottleneck in your experimentation stack.

**Adam Fishman** emphasizes the cultural dimension — experimentation culture requires psychological safety to run tests that might fail, and leadership that celebrates learning from negative results, not just wins.

**Jackson Shuttleworth's Duolingo model (600+ experiments on streaks over 4 years)** offers a high-velocity example: his team runs roughly one experiment every other day, ranging from copy changes to core mechanic redesigns. Key practices: (1) shipping neutral experiments is generally wrong — adds cognitive load without benefit; the exception is when the neutral experiment is a platform for future wins; (2) even wins should sometimes not be shipped — a winning experiment in a sacred space (e.g., the in-lesson experience) may have long-term strategic costs that outweigh short-term gains; (3) copy testing is systematically underrated — the cost is near-zero and some of the biggest retention wins come from changing a few words.

**Itamar Gilad (GIST model)** provides the conceptual backbone for *why* experimentation culture matters: the [[confidence-meter]] makes explicit that all ideas start at near-zero confidence, and only earn investment through staged evidence. Experimentation is not a tool for testing product changes — it's the *default mode* for idea validation at every stage.

**Ronny Kohavi's hard data** adds the empirical foundation that other accounts assume. Across Amazon (~50% failure rate), Microsoft (~66%), Bing (~85%), and Airbnb search (~92%), the universal pattern is that most ideas fail. Three implications for culture: (1) **celebrate negative results** — they are statistically more common than wins and equally informative; (2) **ship nothing flat** — a neutral result means you added code and maintenance burden with zero value; (3) **build institutional memory** — quarterly reviews of the most surprising results prevent the wheel from being reinvented.

Ronny also adds the **OEC (Overall Evaluation Criterion)** discipline: the most common experimentation failure mode is optimizing the wrong metric. Teams must define a metric causally predictive of lifetime value, with countervailing guardrail metrics that prevent short-term wins at the cost of long-term user health.

The **trust dimension** is Kohavi's distinctive contribution: experimentation platforms are safety nets and oracles — they only work if the organization trusts the results. Platforms that produce inflated false positive rates (e.g., early Optimizely's real-time P-value monitoring) destroy the organization's ability to learn from experiments, because results become disconnected from reality.

## Sources

- [[albert-cheng]] — "1,000 experiments/year at Chess.com — the number is a forcing function for investing in tooling and culture"
- [[adam-fishman]] — Key elements of experimentation culture: growth model, instrumentation, no-code tools, cross-functional testing, socialization of learnings
- [[jackson-shuttleworth]] — "600+ experiments on Duolingo streaks; copy testing systematically underrated; neutral experiments usually not worth shipping"
- [[itamar-gilad]] — "Confidence meter; staged validation steps; experimentation as default mode for product development"
- [[ronny-kohavi]] — "The ultimate guide to A/B testing"; 66–92% failure rates across Microsoft/Bing/Airbnb; OEC discipline; Twyman's Law; sample ratio mismatch; trust as foundational to experimentation platforms

## See Also

- [[reverse-free-trial]]
- [[product-market-fit]]
- [[ai-non-determinism]]
