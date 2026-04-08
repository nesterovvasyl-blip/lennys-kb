---
guest: Sander Schulhoff
role: AI researcher; founder of LearnPrompting.org and HackAPrompt; CEO of HackAPrompt
episode: "AI prompt engineering in 2025: What works and what doesn't | Sander Schulhoff"
date: 2025-06-19
topics: [ai, prompt-engineering, llm, security, product-development]
---

# Sander Schulhoff

> The OG prompt engineer — creator of the first prompt engineering guide on the internet, founder of HackAPrompt (the world's biggest AI red-teaming competition), and co-author of The Prompt Report, a 76-page meta-analysis of 1,500+ papers and 200 prompting techniques.

## Background

Sander Schulhoff created the first prompt engineering guide on the internet two months before ChatGPT's release (October 2022). He then partnered with OpenAI to run HackAPrompt — the world's first and now largest AI red-teaming competition, which collected 600,000 adversarial prompts and won Best Theme Paper at EMNLP 2023 (top NLP conference, out of ~20,000 submissions). He co-authored The Prompt Report with OpenAI, Microsoft, Google, Princeton, Stanford, and others. He teaches a Maven course on AI red teaming.

### Is Prompt Engineering Dead?

No. Sander introduces the concept of **artificial social intelligence** — the skill of communicating effectively with AIs, understanding their responses, and adapting accordingly. Studies have shown bad prompts can get 0% accuracy on tasks where good prompts achieve 90%. Models will always be said to have "made it obsolete" but never do.

He distinguishes two modes of prompt engineering:
1. **Conversational**: everyday chatbot interactions where you iterate in real time ("make it more formal," "add a joke")
2. **Product-focused**: building one optimized prompt that runs millions of inputs — the high-value engineering work

Most research and most performance gains come from product-focused prompting. Sander's personal conversational prompting is informal ("writ emil, make better, improve"). The investment in technique pays off at scale.

### Five Core Prompting Techniques

**1. Few-shot prompting** (highest impact, most accessible)
Give examples of what you want. Paste 3–5 samples of the target format/style, then ask for the new output. This is the single most impactful technique for most tasks.

Formatting: use common, consistent formats (XML tags, Q/A pairs). LLMs are trained on common formats, so those formats elicit better responses empirically.

**2. Decomposition**
Ask: "What are the subproblems that need to be solved before you can answer this question?" Then solve each subproblem in sequence. Particularly powerful in multi-step agentic product flows (e.g., a car dealership agent needs to confirm customer identity, car type, date of purchase, and return policy before making a return decision).

**3. Self-criticism**
Ask the LLM to critique its own response, then implement the critique. Run this 2–3 times. Free performance boost; works for both conversational and product-focused use.

**4. Additional information / context**
Provide as much relevant background as possible — company profile, personal biography, research definitions, domain knowledge. Put it at the **beginning** of the prompt, not the end (enables caching; prevents the model from "forgetting" its original task). Don't over-engineer format here; just paste what's relevant.

**5. Ensembling** (advanced)
Pose the same question to multiple prompts, models, or personas; take the most common answer. "Mixture of Reasoning Experts" is a specific implementation. Useful where accuracy matters and cost/latency allow for multiple calls.

### What Doesn't Work Anymore

**Role prompting for accuracy tasks**: Telling the LLM "you are a math professor" does not improve accuracy. Studies found 0.01 accuracy differences — not statistically significant. Modern RLHF-trained models already "self-role" appropriately. Role prompting is still useful for **expressive tasks** (writing in a style, adopting a persona) but not for accuracy-based tasks.

**Threatening or rewarding**: "You'll die if you get this wrong" / "I'll tip you $5" — no strong evidence this works at scale on modern models.

**Chain-of-thought prompting with reasoning models (o3, etc.)**: Already baked in. Still worth including "write out all your reasoning" for non-reasoning models at scale to prevent the rare case where it skips it.

### Actionable Advice
- Start with few-shot prompting and context/additional information — highest uplift, most accessible.
- For product-focused prompting, put additional information at the beginning of the prompt for caching benefits.
- Don't bother with role prompting for accuracy tasks on modern models.
- Use decomposition for complex multi-step reasoning tasks.
- Self-criticism is a free performance boost worth building into product pipelines.
- The best way to improve at prompting is trial and error — more than courses or reading.

### Notable Quotes
> "Studies have shown that using bad prompts can get you down to 0% on a problem, and good prompts can boost you up to 90%."

> "People will always be saying prompt engineering is dead... but then the next model comes out and it's not."

> "The most important places to use these techniques is the product-focused prompt engineering. That is the biggest performance boost."

## Sources
- [[sander-schulhoff]] — "AI prompt engineering in 2025: What works and what doesn't"

## See Also
- [[sander-schulhoff-20]] — AI security episode
- [[prompt-engineering]] (concept)
- [[prompt-injection]] (concept)
- [[ai-evals]]
