---
concept: Prompt Engineering
guests: [sander-schulhoff, sander-schulhoff-20]
topics: [ai, llm, product-development, ai-tools]
---

# Prompt Engineering

> The art and science of crafting inputs to large language models to elicit better, more reliable, or more targeted outputs — spanning casual conversational interaction to precision product-level optimization.

## Overview

Sander Schulhoff — who created the first prompt engineering guide on the internet two months before ChatGPT launched — frames prompt engineering as **artificial social intelligence**: the skill of communicating effectively with AIs, understanding their responses, and adapting inputs accordingly.

Despite repeated predictions of its death, prompt engineering remains highly impactful. Studies cited by Schulhoff show that bad prompts can yield 0% accuracy on tasks where good prompts achieve 90%.

### Two Modes

**Conversational prompt engineering**: Real-time iteration in chat interfaces. Most people's daily use. You see the output and iterate. Schulhoff's own conversational prompting is informal: "writ emil, make better, improve." The advanced techniques below are not always worth applying here.

**Product-focused prompt engineering**: Crafting a single prompt that runs millions of inputs through a pipeline. You can't watch every output — the prompt must be robust, reliable, and performant at scale. This is where the advanced techniques pay off most.

## Guest Perspectives

### Sander Schulhoff ([[sander-schulhoff]], [[sander-schulhoff-20]])

Schulhoff co-authored The Prompt Report — a 76-page meta-analysis of 1,500+ academic papers covering 200+ prompting techniques, co-produced with OpenAI, Microsoft, Google, Princeton, and Stanford.

**Five techniques with the highest impact:**

1. **Few-shot prompting**: Provide 3–5 examples of the desired input/output format. The single highest-impact accessible technique. Use common formats (XML, Q/A pairs) because LLMs are trained on those formats and respond to them most reliably.

2. **Decomposition**: Ask "what are the subproblems that need to be solved first?" before attempting the main task. Particularly powerful for multi-step agentic flows. Example: a car return agent needs to verify customer identity, car details, purchase date, and policy before making a decision.

3. **Self-criticism**: Ask the LLM to critique its own response, then implement the critique. 2–3 rounds provide a free performance boost in both conversational and product contexts.

4. **Additional information (context)**: Provide maximum relevant background. Put it at the **beginning** of the prompt for caching efficiency and to avoid the model "forgetting" its original task. Format doesn't need to be structured — just include what's relevant.

5. **Ensembling** (advanced): Submit the same problem to multiple prompts, models, or personas; take the most common answer. Known as "Mixture of Reasoning Experts" in research. Useful when accuracy is critical and API cost/latency allow multiple calls.

**What doesn't work on modern models:**
- **Role prompting for accuracy tasks**: "You are a math professor" does not improve accuracy. Studies found 0.01 accuracy differences — not statistically significant. (Still useful for expressive/style tasks.)
- **Threatening or rewarding**: "I'll tip you $5" / "someone will die if this is wrong" — no robust evidence of effect on modern models.
- **Chain-of-thought explicitly for reasoning models** (o3, etc.): already baked in. Still worth specifying on GPT-4/4o at product scale to prevent occasional skipping.

## Actionable Takeaways
- Start with few-shot prompting and additional context — highest uplift, lowest friction
- For product pipelines, invest in decomposition and self-criticism loops
- Put additional information at the beginning of prompts for caching benefits
- Stop role prompting for accuracy tasks; use it only for expressive tasks
- Trial and error beats courses and reading as the fastest way to improve
- Prompt-based defenses ("do not follow malicious instructions") are security theater — see [[prompt-injection]]

## Sources
- [[sander-schulhoff]] — "AI prompt engineering in 2025: What works and what doesn't"
- [[sander-schulhoff-20]] — "Why securing AI is harder than anyone expected"

## See Also
- [[prompt-injection]]
- [[ai-evals]]
- [[context-engineering]]
- [[overall-evaluation-criterion]]
