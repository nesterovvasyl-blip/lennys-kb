---
author: Hamel Husain, Shreya Shankar
guests: [hamel-husain, shreya-shankar]
---

# Open Coding / Error Analysis for AI Products

> A structured qualitative analysis method borrowed from social science — used to systematically discover, categorize, and prioritize failure modes in LLM-based products before building automated evaluators.

## Content

Developed and popularized for AI product development by [[hamel-husain]] and [[shreya-shankar]] in their Maven course "AI Evals for Engineers and Product Managers." The methodology adapts grounded theory techniques from social science qualitative research to the problem of understanding what's wrong with an AI application's outputs.

**Why before automated evals**: Most teams want to skip straight to automated testing. The problem: automated evaluators measure what you tell them to measure. If you don't know what failure modes exist in your actual production outputs, you'll build evaluators for the failure modes you imagined — which often aren't the ones that are actually happening. Open coding tells you what to measure. Automated evals measure it at scale.

**Step 1: Open Coding**
Pull 50-100 real traces (production conversations or outputs) from your system. For each trace, read it carefully and write a first-error note in plain language. Rules:
- Be specific and descriptive, not vague ("Did not confirm call transfer before executing it" not "bad")
- Write what happened, not what should happen
- Don't try to categorize yet — just describe
- One note per trace (just the first/most important error if there are multiple)
- Use enough words that an LLM could categorize it later

Hamel's real-world example: a property management AI assistant that was supposed to handle leasing inquiries. Open codes included things like "Did not confirm call transfer with user," "Answered question about floors that isn't in our system," "Abruptly ended conversation without resolution."

**Step 2: Generate Axial Codes**
After collecting 50-100 open codes, use an LLM (Claude, ChatGPT, etc.) to cluster them into axial codes — categories of failure modes. Prompt: "I have a set of open codes from manual trace review. Please analyze them and generate axial codes (failure mode categories) that organize them. Here are the codes: [CSV or list]."

The LLM will produce a first draft. Iterate on it — make the categories specific and actionable, not generic (not "capability limitations" but "incorrect handling of human escalation requests").

**Theoretical saturation** (from [[shreya-shankar]]): Stop collecting open codes when you're no longer discovering new types of problems. For most products, saturation happens between 40-150 traces. 100 is a useful starting target.

**Step 3: Assign Axial Codes to Traces**
Use an LLM + spreadsheet to automatically assign each trace to one of your axial codes. Include a "none of the above" category — when the LLM can't categorize a trace, your taxonomy has a gap. Iterate until coverage is good.

**Step 4: Count and Prioritize**
Use a pivot table (or equivalent) to count occurrences of each failure mode. Now you have data: "17 conversational flow issues, 8 human handoff failures, 12 formatting errors." Some failures are frequent; some are rare but critical. Prioritize based on both frequency and business impact.

**Step 5: Decide what to fix**
For each failure mode:
- **Simple prompt fix**: Some failures reveal you just didn't specify the behavior in the system prompt. Fix the prompt. You may not need an eval for this.
- **LLM-as-judge eval**: For complex, judgment-based failure modes (e.g., "appropriate human escalation"), build a binary [[llm-as-judge]] evaluator.
- **Code-based eval**: For mechanical failure modes (output format, length, specific vocabulary), write a code-based check.

**The ongoing cycle**: After building LLM-as-judge evaluators, run them continuously on production samples. Monitor failure rates as a product health metric. Re-do open coding quarterly or when the product changes significantly.

## Sources
- [[hamel-husain]] — "The first thing I do with every client is look at their traces. It always teaches us everything." (How to evaluate AI products, 2025)
- [[shreya-shankar]] — "You can't dream up your failure modes before you see your data. Criteria drift is real." (Who Validates the Validated?, 2025)

## See Also
- [[hamel-husain]]
- [[shreya-shankar]]
- [[ai-evals]]
- [[llm-as-judge]]
- [[ai-products]]
