---
aliases: [evals, evaluations, ai-evaluations, rlhf]
guests: [brendan-foody, hamel-husain, shreya-shankar, karina-nguyen, nick-turley]
---

# AI Evals

> Evaluation datasets and rubrics that define what "success" looks like for a model capability — the prerequisite for all post-training improvement.

## Content

"Evals" (short for evaluations) are the systematic way to measure what good model output looks like for a specific capability domain. They sit at the center of modern AI development — used for post-training (reinforcement learning), benchmarking model progress, and as sales collateral for demonstrating model capabilities.

### Why Evals Matter: The PRD Analogy

Brendan Foody's core framing: "If the model is the product, then the eval is the PRD." Labs run dozens of experiments per day where they make small improvements toward an eval set. Reinforcement learning is so effective that once a high-quality eval exists, models can climb it rapidly — as demonstrated by how quickly models saturated Olympiad Math and SWE-bench benchmarks once those evals were focused on.

The limiting factor for frontier model improvement is no longer compute or architecture — it is the ability to measure what "good" looks like across every new domain. "Evals are all you need" (Greg Brockman / OpenAI). "Models are only as good as their evals" (common Mercor customer quote).

### What Writing an Eval Actually Looks Like

A lawyer being asked to eval a contract red-lining model would:
1. Create a rubric (like a professor creating criteria for a deliverable): what are the key things the model should identify and how should they be weighted?
2. Score model outputs against this rubric (similar to a TA applying professor criteria to student work)
3. Use this as both a benchmark (has the model improved?) and training signal (reward model trajectories that score higher)

This is the "human defined success criteria" approach that powers modern RLHF and its successor, reinforcement learning from AI feedback (RLAIF), where models are increasingly used to score other models once the rubric is established.

### The Shift from Crowdsourced to Expert Labor

The AI data market has fundamentally shifted. Early RLHF relied on crowdsourced platforms (Scale AI, Surge) using high volumes of lower-skilled workers to provide relative preference judgments ("which response is better?"). The current paradigm requires domain experts who can:
- Write rubrics from deep domain knowledge
- Create hard problem sets that expose model gaps
- Evaluate complex professional outputs (contract analysis, medical diagnosis, financial modeling)

Mercor's business (Brendan Foody) is built on sourcing these experts — Goldman bankers, doctors, McKinsey analysts, Harvard Lampoon comedy writers, Emmy-winning screenwriters. The top 10% of contributors drive the majority of model improvement.

### Evals as the New Marketing

Sarah Guo (AI investor) coined "evals equal your new marketing." Because evals are the measure of model capabilities, releasing strong eval performance is how labs demonstrate competitiveness to customers, researchers, and developers. The move is from academic benchmarks (GPQA, Humanity's Last Exam) to domain-specific practical capabilities benchmarks (how well does the model do investment banking analysis?).

### For Enterprises

The practical advice for enterprises: build a systematic way to measure how well AI automates your core value chain. "Each company has its own value chain or maybe a handful of them if it's a multi-product company. Just thinking about how they measure that is the prerequisite to really effectively applying AI throughout their entire business." (Foody)

An architecture firm needs to eval how well AI produces architecture diagrams. A bank needs to eval investment analysis quality. Without this measurement infrastructure, any AI deployment is flying blind.

### Durability

Foody's view on timeline: evals are evergreen. "So long as we want to improve models, we'll need experts to create evals for them and to create the post-training data for them to learn those capabilities." Even if we reach a point where many workflows are automated, the frontier of what models can't yet do will continue to expand, and those new domains will require new evals.

### The Practitioner Methodology: Open Coding → Axial Coding → LLM Judges

[[hamel-husain]] and [[shreya-shankar]] bring a complementary perspective focused on product-level evals for LLM applications — not foundation model training, but the ongoing measurement and improvement of deployed AI products. Their methodology is grounded in social science qualitative research:

**Error analysis first**: Before writing any automated evaluator, manually review 50-100 real production traces. Write a plain-language "open code" note for each (e.g., "Did not confirm call transfer before executing it"). This step — which most teams skip — reveals what's actually failing, which is often different from what you imagined would fail. This is what Shreya calls "criteria drift": your definition of good output changes as you see real failure modes you never anticipated.

**Axial coding**: After collecting open codes, use an LLM to cluster them into categories (axial codes). Iterate until the categories are specific and actionable. Use a "none of the above" option to detect gaps in your taxonomy.

**Theoretical saturation**: Stop reviewing traces when you're no longer discovering new types of failures. This is the principled stopping rule from qualitative social science. Most products saturate between 40-150 traces.

**Binary LLM-as-judge**: For failure modes that can't be caught by code checks, build a binary (pass/fail) LLM evaluator. Validate it against your human annotations using a confusion matrix. Reject evaluators that only report aggregate agreement; check false positive and false negative rates separately.

**Continuous monitoring**: Run LLM-as-judge evaluators continuously on sampled production traces (e.g., 1000 per day). This gives you a real-time quality dashboard, not just a pre-release gate.

**The meta-point**: Hamel and Shreya argue that evals are fundamentally just data science applied to AI products — not a new discipline. Error analysis, A/B tests, user feedback, LLM judges, dogfooding — all are tools in the same analytical toolkit. The "evals vs. vibes" debate reflects vocabulary confusion, not a real disagreement about the underlying practice of rigorous measurement.

Their course on Maven is the highest-grossing course on the platform. They also maintain a 160-page reference book and a trained AI bot that answers questions about evals methodology. See [[open-coding-error-analysis]] for the full step-by-step framework.

### Evals as the New PRD: The Product Builder Perspective

[[karina-nguyen]] (AI researcher at OpenAI, formerly Anthropic) provides a complementary inside-the-lab view of how evals function in product development — not just foundation model training, but building AI-native product features.

At OpenAI, product development for AI features like Canvas and Tasks begins by defining what "correct behavior" looks like in concrete pass/fail terms. Product managers and model designers write spreadsheets with three columns: current behavior, ideal behavior, and why. This document serves simultaneously as an eval dataset and potential training data. The intuition: "If you can't define correct, you can't build or improve the feature."

This is Karina's restatement of the PRD analogy from the product side: traditional product specs describe what to build; eval specs describe what good looks like. For AI features, the latter is more powerful — because once you can reliably measure "good," reinforcement learning can generate the behaviors without exhaustive human-written rules.

Her process for new AI features:
1. Identify 2-3 core behaviors you want the model to exhibit
2. Use a capable model (like o1) to generate diverse synthetic conversations representing those behaviors
3. Build deterministic evals to measure pass/fail on each behavior
4. Launch, collect user feedback, iterate on both synthetic data and evals

This process enabled Canvas to go from zero to shipped in 4-5 months. The feedback loop speed comes from synthetic data being cheap to generate and easy to adjust post-launch based on real user behavior.

### Nick Turley (OpenAI / ChatGPT)

Turley offers a product leader's perspective on evals from inside OpenAI. He started writing evals before he knew what an eval was — he was simply outlining "very clearly specified ideal behavior for various use cases" in documents. When a researcher told him "you should make an eval," he realized there was an entire research discipline that mapped to what product people call success criteria.

His reframe: evals are not some technical magic requiring ML expertise. "It's really just about articulating success in a way that is maximally useful for training models. It's not that different from the wisdom of, 'You ought to articulate success before you do anything else.' It's just a new mechanism for doing that." You can write evals in a spreadsheet.

His core advice for PMs: writing evals is the new lingua franca for communicating what a product should do to ML teams. PMs who understand this — that defining success and communicating it as testable behavior — become far more effective at product development in AI environments. "I hope to demystify it for people who hear that term."

## Sources
- [[brendan-foody]] — "If the model is the product, then the eval is the PRD." (Why experts writing AI evals is creating the fastest-growing companies in history)
- [[hamel-husain]] — "The first thing I do with every client is look at their traces. It always teaches us everything." (How to evaluate AI products, 2025)
- [[shreya-shankar]] — "You can't dream up your failure modes before you see your data." (How to evaluate AI products, 2025)
- [[karina-nguyen]] — "The cost of reasoning and intelligence is drastically going down." (OpenAI researcher on why soft skills are the future of work, 2025-02-09)
- [[nick-turley]] — "It's really just about articulating success in a way that is maximally useful for training models." (Inside ChatGPT: The fastest growing product in history, 2025-08-09)

## See Also
- [[brendan-foody]]
- [[hamel-husain]]
- [[shreya-shankar]]
- [[open-coding-error-analysis]]
- [[ai-products]]
- [[outcomes-based-pricing]]
