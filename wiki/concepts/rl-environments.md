---
aliases: [reinforcement learning environments, AI training environments, RL]
guests: [edwin-chen]
---
# RL Environments

> Simulated real-world scenarios used to train AI models through reinforcement learning — the next phase of post-training after SFT, RLHF, and rubrics/verifiers.

## Content

Edwin Chen at Surge AI describes RL environments as "the hot new thing" in AI post-training as of 2025-2026. The idea: instead of training on human feedback on isolated tasks, put AI models in a fully realized simulated world and reward or penalize them based on how well they complete end-to-end tasks over long time horizons.

### The Evolution of AI Post-Training

Edwin describes four progressive stages, each a different human learning analogy:

1. **SFT (Supervised Fine-Tuning)** — "Like mimicking a master and copying what they do." Give the model good examples; it learns to reproduce them.

2. **RLHF (Reinforcement Learning from Human Feedback)** — "Like writing 55 different essays and someone telling you which one they liked the most." Train the model to predict human preferences.

3. **Rubrics and Verifiers** — "Like learning by being graded and getting detailed feedback on where you went wrong." Evaluators give structured, detailed feedback on specific dimensions.

4. **RL Environments** — "Like building a video game with a fully fleshed out universe." Models operate in complex simulated environments, with rewards tied to completing realistic multi-step tasks.

These stages are complementary, not mutually exclusive — each new stage adds a different form of learning on top of previous ones.

### What an RL Environment Looks Like

A Surge-built example: a startup with Gmail messages, Slack threads, Jira tickets, GitHub PRs, and a full codebase. "Suddenly AWS goes down. And Slack goes down. Model, what do you do?"

The model must navigate confusing information, use tools it may not have seen before, and take actions where step 1 affects step 50. This is completely unlike single-step academic benchmarks.

A financial analyst environment: a Bloomberg terminal, a spreadsheet, calculation tools. Goal: "Does cell B22 contain the correct P&L number?" The model must learn to use each tool correctly, sequentially, over a long trajectory.

### Why Trajectories Matter

Even when models reach the correct final answer, they may do so through wasteful or broken paths — trying 50 things and randomly landing on the answer, or reward-hacking to get the correct number through a shortcut. Training on trajectories (not just outcomes) teaches models to get there *correctly and efficiently*.

### Why RL Environments Reveal Model Weaknesses

Models that score well on academic benchmarks often "fail catastrophically" in RL environments — because real-world tasks are messy, ambiguous, and multi-step. "You have all these models that seem really smart on isolated benchmarks, they're good at single-step tool calling. But suddenly you dump them into these messy worlds where you have confusing Slack messages and tools they've never seen before."

### Implications

Edwin believes we need a "suite of products that reflect a million different ways that humans learn" — and RL environments are one critical piece. Just as a great writer doesn't improve by memorizing grammar rules but by reading great books, practicing, getting feedback, and developing taste over years, models need diverse, rich learning experiences.

## Sources

- [[edwin-chen]] — "The $1B AI company training ChatGPT, Claude & Gemini on the path to responsible AGI"

## See Also

- [[ai-evals]]
- [[world-models]]
- [[ai-non-determinism]]
