---
guest: Shreya Shankar
role: PhD Researcher; Course instructor "AI Evals for Engineers and PMs"
episode: "How to evaluate AI products: A deep dive into evals | Hamel Husain & Shreya Shankar"
date: 2025-03-06
topics: [ai-evals, ai-products, data-science, research, llm-applications]
---

# Shreya Shankar

> PhD researcher and co-creator of the leading practical curriculum on AI evals, known for applying rigorous social science methodology to the problem of evaluating LLM applications — and for writing the paper "Who Validates the Validators?" on the underappreciated challenge of criteria drift.

## Content

Shreya Shankar is a PhD researcher with a background in machine learning and data science. She co-created (with [[hamel-husain]]) the Maven course "AI Evals for Engineers and Product Managers," which has become the platform's highest-grossing course. Her research focuses on practical methodology for measuring AI product quality, drawing on social science qualitative analysis techniques that most AI practitioners have never encountered. She authored the paper "Who Validates the Validated?" documenting the phenomenon of criteria drift in AI evaluation.

This was a joint episode with [[hamel-husain]].

### Key Ideas

- **Criteria drift — why evals fail**: Shreya's landmark insight from her research paper "Who Validates the Validated?": people's definitions of "good" change as they review more AI outputs. You start with a rubric, but after seeing 10 edge cases you never anticipated, your understanding of what the product should do has evolved. This means evaluation rubrics written before looking at data are almost always wrong. The practical implication: don't write your evals before looking at your data. Look first, discover what you care about, then formalize.

- **Theoretical saturation as the stopping rule**: Borrowed from qualitative social science research, theoretical saturation is the principled answer to "how many traces do I need to review?" — stop when you're no longer discovering new types of problems. For most AI products, Shreya and Hamel recommend starting with 100 (as a psychological unblocking number), but the real criterion is when you're saturated. Some products saturate at 40; complex ones might need 200+.

- **Axial coding — organizing open codes into categories**: After open coding (writing a first-error note per trace), the raw notes are noisy. Axial coding is the process of clustering open codes into actionable categories. An LLM can do the first draft of axial codes, but the human needs to review, iterate, and rename them until they're specific and actionable (not "capability limitations" which is too vague, but "did not confirm call transfer with user" which tells you exactly what to fix).

- **"None of the above" in LLM judge prompts**: When using an LLM to assign axial codes to traces, Shreya recommends always including a "none of the above" category. When the judge assigns "none of the above," it's a signal that your taxonomy is incomplete — there are failure modes you haven't categorized yet. This prevents the LLM from force-fitting every trace into an existing category and hiding gaps in your analysis.

- **Evals as continuous product improvement, not one-time testing**: A common misconception: evals are tests you run before shipping. Shreya's framing is that evals should run continuously on production traces — sampling 1,000 real interactions daily, running LLM-as-judge evaluators, tracking failure rate metrics over time. This gives you a real-time quality dashboard, not just a pre-release gate. The companies doing this well don't talk about it publicly — it's a competitive moat.

- **Evals are all data science**: Shreya's meta-framing echoes Hamel's: the evals debate is a distraction from the underlying truth that building great AI products requires data science thinking. Error analysis, A/B tests, LLM judges, monitoring dashboards — these are all variants of "measure what's happening, understand why, improve it." The tools are the same. The "evals vs. vibes" debate is usually a misunderstanding about scope and vocabulary.

- **Cost optimization through model tiering**: For teams whose eval infrastructure is working but expensive, Shreya covers how to replace expensive frontier model calls (GPT-4, Claude Opus) with smaller, cheaper models (GPT-4-mini, Claude Haiku) for specific evaluation tasks once you've validated the smaller model gives equivalent results. This can cut eval infrastructure costs dramatically while maintaining quality.

### Actionable Advice

- Before writing any evaluation criteria, look at 50-100 real outputs from your product. Let your criteria emerge from the data, not your initial assumptions.
- Include "none of the above" in any LLM classification prompt you use for axial coding. It's your quality signal that the taxonomy is incomplete.
- Build a weekly 30-minute trace review habit. After the initial 3-4 day setup investment, ongoing maintenance is fast and the improvement rate is high.
- When someone shows you an LLM judge that "agrees 75% of the time," ask for the confusion matrix. Check false positive vs. false negative rates separately — aggregate agreement can mask systematic failures.

### Notable Quotes

> "You can't dream up your failure modes before you see your data. People's definitions of 'good' change as they review outputs. That's criteria drift."

> "Theoretical saturation is when you're not uncovering any new types of problems. That's when you stop coding. Not at 100 — but 100 is a good mental unblock."

> "I want product managers to be able to build profitable AI products. We are definitely not the only two people who should be teaching this."

## Sources
- [[shreya-shankar]] — "How to evaluate AI products: A deep dive into evals" (2025)

## See Also
- [[hamel-husain]]
- [[ai-evals]]
- [[open-coding-error-analysis]]
- [[llm-as-judge]]
- [[ai-products]]
