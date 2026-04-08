---
framework: DORA Metrics
created_by: Nicole Forsgren
guests: [nicole-forsgren]
date_added: 2026-04-08
---

# DORA Metrics

> Four key metrics for measuring the speed and stability of a software delivery pipeline — the most widely adopted framework for engineering productivity, now needing careful interpretation in the age of AI.

## Overview

DORA (DevOps Research and Assessment) metrics were developed by Nicole Forsgren and her research team. They represent the four key indicators that best predict both software delivery performance and organizational performance. The research behind them is detailed in the book *Accelerate*.

DORA is a prescriptive metric set — meaning it should be used only for the purpose for which it was designed: assessing the speed and stability of the software delivery pipeline. It is not a general-purpose productivity framework.

## Components / Steps

**Speed Metrics:**
1. **Deployment Frequency** — How often do you deploy to production? (Elite: multiple times per day)
2. **Lead Time for Changes** — How long does it take from code commit to code running in production? (Elite: less than one hour)

**Stability Metrics:**
3. **Mean Time to Recovery (MTTR)** — How long does it take to recover from a production failure? (Elite: less than one hour)
4. **Change Failure Rate** — What percentage of deployments cause failures requiring rollback or hotfix? (Elite: 0-15%)

## Application

DORA is best used as a pipeline health check. High-performing organizations consistently score better on all four dimensions, and this correlates strongly with both organizational performance and developer wellbeing.

**What DORA is good for:**
- Benchmarking your delivery pipeline against industry standards
- Identifying systemic bottlenecks (if lead time is high, where is time being lost?)
- Tracking directional improvement over time

**What DORA is NOT good for (especially post-AI):**
- Measuring individual developer productivity
- Capturing the new feedback loops AI tools create earlier in the pipeline (pre-commit, mid-development)
- Understanding code quality, developer satisfaction, or innovation capacity

## DORA in the AI Era

Nicole Forsgren cautions that DORA cannot be blindly applied in 2025. AI has created new feedback loops throughout the development process that DORA wasn't designed to capture. The traditional DORA loop assumed feedback came primarily from production; now feedback is available at every stage of development, often in real time.

Additionally, AI tools that generate large amounts of code can make deployment frequency and lead time look better while masking quality issues. Metrics like code survivability rate (how much AI-generated code persists over time without modification) and code quality distribution (human vs. machine) are emerging as important complementary measures.

Use DORA for what it was designed: pipeline speed and stability assessment. Pair it with [[SPACE framework]] for a more complete picture of developer experience.

## How to Apply

1. **Start with listening** before picking metrics — survey developers about their top 3 friction points and how frequently each affects them
2. **Pick metrics that map to what leadership cares about**: market share → speed; profit margin → costs; transformation → velocity
3. **Use DORA** to establish a pipeline performance baseline; track improvements to deployment frequency and lead time as DevEx work compounds
4. **Track code survivability rate** (how much AI-generated code persists vs. is replaced) as a new quality signal
5. **Re-evaluate metrics** as AI changes what's important — some metrics should be sunset when they no longer drive decisions

## Sources

- [[guests/nicole-forsgren]] — "How to measure AI developer productivity in 2025" (Lenny's Podcast, 2025-10-19)

## See Also

- [[frameworks/space-framework]]
- [[concepts/developer-experience]]
- [[concepts/velocity]]
