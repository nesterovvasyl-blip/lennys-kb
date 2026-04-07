---
guest: Hamel Husain
role: AI consultant and educator; Course instructor "AI Evals for Engineers and PMs"
episode: "How to evaluate AI products: A deep dive into evals | Hamel Husain & Shreya Shankar"
date: 2025-03-06
topics: [ai-evals, ai-products, data-science, product-development, llm-applications]
---

# Hamel Husain

> AI consultant and educator who has turned error analysis and evaluation methodology into the clearest practical curriculum for building better AI products — co-creator (with Shreya Shankar) of the leading Maven course on AI evals.

## Content

Hamel Husain is an independent AI consultant and educator with a background in machine learning, data science, and software engineering. He has worked with numerous companies on deploying and improving LLM-based applications, and he co-created (with [[shreya-shankar]]) a Maven course called "AI Evals for Engineers and Product Managers" that has become the highest-grossing course on the Maven platform. His practical philosophy: before writing a single automated eval, you must manually look at your data — this step alone is the highest-ROI activity for improving AI products.

This was a joint episode with [[shreya-shankar]].

### Key Ideas

- **Look at your traces first — always**: Hamel's most repeated advice: before building automated evals, before writing LLM-as-judge prompts, before any of the sophisticated stuff — look at 50-100 actual traces (conversations, completions, outputs) from your system manually. He does this with clients immediately. "Let's go look at your traces right now." The people who are shocked by this have never done it; the people who have done it are shocked they ever went without. This is where you discover what's actually happening, not what you think is happening.

- **Open coding: the error analysis process**: The Hamel/Shreya methodology borrows from social science qualitative research. Step 1: open coding — read traces one at a time, write a brief first-error note in plain language about what went wrong ("Did not confirm call transfer with user," not "jank"). Be specific enough that an LLM could categorize it later. Step 2: after 50-100 traces, collect all notes, use an LLM to generate axial codes (categories of failure modes). Step 3: iterate on the categories until they're specific and actionable. Step 4: build automated evaluators only for the failure modes that persist after simple prompt fixes.

- **Benevolent dictator for eval criteria**: When a team debates what "good" looks like in an AI product output, the debate can be infinite. Hamel's solution: designate a single trusted domain expert as the "benevolent dictator" — the one person whose judgment about quality is authoritative. Not a committee, not a vote. The domain expert (often the PM, sometimes a subject matter expert) makes the call. This creates a coherent standard against which everything else is measured.

- **Binary LLM-as-judge, not Likert scale**: A common mistake is using 1-5 or 1-7 scales for LLM-as-judge evaluations. "My judge gives an average of 4.2" — meaningless. What does 4.2 vs. 3.7 mean? Hamel advocates binary (pass/fail) judges for every specific failure mode. Painful to define, but the resulting metric is unambiguous and actionable. Before deploying an LLM judge, validate it against your own human annotations: create a confusion matrix, check both false positive and false negative rates.

- **Theoretical saturation as the stopping rule**: The question of "how many traces should I look at?" has a principled answer from qualitative social science: keep looking until you reach theoretical saturation — the point at which you're not discovering new types of problems. In practice, Shreya and Hamel recommend targeting 100 traces as a mental frame (not too intimidating, usually enough), with the understanding that you'll naturally keep going once you see how much you learn.

- **Evals as data science, not a separate discipline**: Hamel's meta-point about the "evals debate": the argument between "do evals" vs. "just vibe and look at your product" is a false dichotomy. Both are forms of data analysis. Error analysis, A/B testing, dogfooding, LLM-as-judge monitoring, user research — all are tools in the same analytical toolkit. The word "evals" creates unnecessary controversy; the underlying practice is just rigorous measurement of product quality.

### Actionable Advice

- Don't buy an eval tool first. Start by opening a spreadsheet, pulling 100 traces, and writing a plain-language first-error note for each one.
- Use open codes in Google Sheets or Notion — they don't need to be software; the structure and habit matter more than the tool.
- Build your own lightweight trace review interface (a simple web app takes a few hours with AI coding tools) to make it easy to review data regularly. Remove all friction from the most important habit.
- When evaluating a junior team member's eval work, ask for the confusion matrix. If they can't produce it, they haven't validated their judge.

### Notable Quotes

> "The first thing I do with every new client is say, 'Let's look at your traces.' Their eyes pop open. They've never done it. It always teaches us everything we need."

> "Don't ask the AI to eval itself. Look at the data. Look at it yourself. It's the highest ROI activity you can do."

> "Binary judges. Pass or fail. If someone reports 4.2 on a seven-point scale, ask them what that means. They won't know."

## Sources
- [[hamel-husain]] — "How to evaluate AI products: A deep dive into evals" (2025)

## See Also
- [[shreya-shankar]]
- [[ai-evals]]
- [[open-coding-error-analysis]]
- [[llm-as-judge]]
- [[ai-products]]
