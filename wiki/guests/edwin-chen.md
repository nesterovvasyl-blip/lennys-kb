---
guest: Edwin Chen
role: Founder and CEO, Surge AI
episode: "The $1B AI company training ChatGPT, Claude & Gemini on the path to responsible AGI | Edwin Chen"
date: 2025-12-07
topics: [ai, growth, startup, leadership, data, metrics]
---
# Edwin Chen

> Founder and CEO of Surge AI, the fastest company ever to reach $1B in revenue (under 4 years, under 100 people, bootstrapped from day one), teaching AI models what is good and bad through elite human data and evaluations.

## Bio

Edwin Chen is a former researcher and engineer at Twitter, Google, and Facebook who founded Surge AI with a radical premise: build a tiny, elite team and stay completely off Silicon Valley's radar. Surge reached $1 billion in revenue in under four years with fewer than 100 employees, never raised VC money, and was profitable from day one. The company powers RLHF, SFT, rubrics, verifiers, and RL environments for every major frontier AI lab — OpenAI, Anthropic, Google DeepMind, and others.

Edwin is deeply contrarian about how AI should be built, how startups should operate, and what the industry is getting wrong about AI progress.

### Key Ideas

- **Small elite teams outperform large ones**: "I always felt that we could fire 90% of the people and we would move faster because the best people wouldn't have all these distractions." Surge proved this at extreme scale — $1B revenue with <100 people. Edwin predicts ratios like $100B per employee will emerge as AI improves.

- **Quality in AI data is not checklist compliance**: Most companies think high-quality training data means checking boxes — is it a poem? Does it have 8 lines? Does it mention the moon? Surge defines quality differently: "Is it Nobel Prize-winning? Is it unique? Full of subtle imagery? Does it surprise you?" This requires building thousands of signals on workers' performance and outputs, similar to how Google Search evaluates webpages — removing the worst and finding the best of the best.

- **Benchmarks are misleading**: Edwin doesn't trust AI benchmarks for two reasons: (1) the benchmarks themselves often have wrong answers, and (2) they have well-defined objective answers that are easy to hill-climb on in ways that don't correlate with real-world performance. "It's kind of crazy that these models can win IMO gold medals but still have trouble parsing PDFs." Companies optimize benchmarks for PR, not for actual capability improvement.

- **AI is heading in the wrong direction**: Edwin's hot take is that labs are optimizing for dopamine-chasing AI — sycophantic, flashy, emoji-heavy responses — because random users on platforms like LLM Arena vote based on superficial cues. "We're basically optimizing your models for the types of people who buy tabloids at the grocery store." Anthropic is the exception: "Anthropic takes a very principled view about what they do and don't care about."

- **Human evaluations over benchmarks**: Surge measures AI progress by running expert human annotators through realistic task scenarios — having a physicist push the frontier of their research with the model, having a coder work through real company problems. These experts verify code, check equations, and evaluate deeply rather than vibing on two-second glances.

- **AGI timeline**: Edwin is in the "longer" camp. He sees a big difference between going from 80% → 90% → 99% AI capability. He estimates within 1-2 years, models will automate ~80% of an L6 software engineer's job; another decade+ to reach 99%. Human annotators aren't going away until actual AGI — by definition, there's always more to learn from humans until that threshold.

- **RL environments as the next frontier**: After SFT (supervised fine-tuning, mimicking a master), RLHF (learning from preferences, like writing essays and seeing which one someone liked), and rubrics/verifiers (detailed feedback like being graded), the next learning paradigm is RL environments — simulated real-world scenarios. Surge builds these: a startup with Gmail, Slack, Jira, GitHub, and then "AWS goes down" — what does the model do? Trajectories matter, not just final outcomes.

- **Build the one thing only you could build**: Edwin's advice to founders rejects the Silicon Valley pivot culture. "Don't pivot. Don't blitz-scale. Don't hire that Stanford grad who wants to add a hot company to their resume. Just build the one thing only you could build."

- **Model personalities will diverge**: A year ago Edwin expected AI models to commoditize. Now he believes company values will permanently shape model behavior — the objective function you optimize for determines the kind of AI you create. Companies that optimize for engagement will get sycophantic models; companies that optimize for truth will get principled ones.

### Actionable Advice

- Don't raise VC money if you can avoid it — it pulls you into a PR hamster wheel and encourages you to optimize for valuation over product.
- Avoid customers who don't deeply understand and care about what you're building in the early days — mission-aligned customers give better feedback.
- Think about AI quality as a two-sided problem: remove the worst of the worst, but also specifically find and reward the best of the best.
- When evaluating AI models, don't use benchmarks as your primary signal — design evaluations that reflect actual real-world tasks.
- Pay attention to model trajectories, not just final outputs. How a model gets to an answer matters as much as whether it gets there.

### Notable Quotes

> "We're basically teaching our models to chase dopamine instead of truth."

> "It's kind of crazy that these models can win IMO gold medals, but they still have trouble parsing PDFs."

> "The easiest way to climb LLM Arena is adding crazy bolding, doubling the number of emojis, tripling the length of your model responses — even if your model starts hallucinating."

> "Just build the one thing only you could build — a thing that wouldn't exist without the insight and expertise that only you have."

> "I would rather be Terrence Tao than Warren Buffett."

## Sources

- [[edwin-chen]] — "The $1B AI company training ChatGPT, Claude & Gemini on the path to responsible AGI"

## See Also

- [[ai-evals]]
- [[product-market-fit]]
- [[startup-resilience]]
- [[ai-non-determinism]]
