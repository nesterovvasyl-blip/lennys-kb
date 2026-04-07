---
aliases: [data labeling, post-training data, RLHF, SFT, human feedback]
guests: [garrett-lord]
---

# AI Training Data

> The human-generated data used to improve frontier AI models through post-training — the fastest-growing and most constrained input in modern AI development.

## Content

As of 2025, AI model improvement has shifted from pre-training (ingesting the public internet) to post-training (targeted augmentation with high-quality, domain-specific data). Garrett Lord (Handshake CEO) provides one of the clearest explanations of this space available, as he built a $100M ARR business serving frontier labs within a year.

### Pre-Training vs. Post-Training

**Pre-training**: Feed the model the entire written corpus of human knowledge — books, websites, videos, code. The model learns language, facts, and general reasoning. Pre-training gains have been asymptoting as labs have exhausted available public internet data.

**Post-training**: Augment and improve the model's capabilities in specific domains through new data creation. This is now where most capability gains come from. It's not a one-time step; labs run it continuously as a research process.

### Types of Post-Training Data

**RLHF (Reinforcement Learning from Human Feedback)**: Preference ranking. Human evaluators compare two model outputs and indicate which is better. Teaches the model what "good" looks like in a domain.

**SFT (Supervised Fine-Tuning)**: Prompt-response pairs where the human expert provides the correct, high-quality answer. The model learns to produce similar answers.

**Trajectories**: Full recordings of how a human expert solves a problem — screen capture, mouse movement, voice narration, tool use. Labs want to model human expert problem-solving in multi-step environments (professional tasks, research processes, complex workflows). The format is typically structured data (JSON).

**Rubrics**: Human-defined evaluation criteria that allow a model to act as a judge on future outputs. Particularly important in subjective domains (educational design, legal writing, medical diagnosis) where there is no single correct answer.

**Breaking and Red-Teaming**: Domain experts actively try to make the model fail — find incorrect reasoning steps, wrong answers, capability gaps in their field. Each failure becomes training data to fix. A physics PhD who can make a frontier model fail in 10 different ways in quantum mechanics provides far more value than a generalist who finds trivial errors.

### The Shift from Generalists to Experts

Early data labeling used low-cost labor for generic tasks (drawing bounding boxes, classifying images, basic text annotation). As models improved, generalist tasks became trivially automatable. Now labs need:

- PhDs and specialists who can extend the frontier of human knowledge in their domain
- Professionals with real-world experience (teachers with classroom insights, accountants with audit expertise)
- People who can navigate multi-step professional workflows (legal research, scientific experimentation, financial analysis)

Expert rates: $100-200/hour for top specialists in advanced STEM fields.

### What Labs Actually Care About

1. **Quality**: Wrong training data is extremely hard to overcome and can degrade model performance in subtle ways. Labs invest heavily in quality assurance.
2. **Volume**: Can you produce thousands of high-quality units of data in a difficult domain? Scale matters for the statistical robustness of improvements.
3. **Speed**: Labs run parallel research experiments. The ability to spin up a data collection pipeline in days and scale it quickly is competitive.

### Competitive Moat in the Data Business

Garrett Lord's insight: "The only moat in human data is access to an audience." Companies without an existing expert community must spend millions on performance advertising (LinkedIn, Instagram, Google) and employ hundreds of recruiters to find qualified experts — who have no reason to trust them. Handshake had a decade of trust with 18M professionals including 500K PhDs, enabling far lower customer acquisition costs and higher completion rates.

### Future Directions

- **Trajectory data** will grow as labs focus on agentic AI that needs to act in the world, not just generate text
- **Professional domain data** (legal, medical, financial) will expand as labs try to make models useful for high-stakes knowledge work
- The constraint of expert availability makes companies with captive expert audiences (universities, professional networks, research institutions) structurally advantaged

## Sources
- [[garrett-lord]] — "Inside the expert network training every frontier AI model" (Lenny's Podcast, 2025-08-24)

## See Also
- [[ai-products]]
- [[rl-environments]]
- [[world-models]]
- [[ai-evals]]
