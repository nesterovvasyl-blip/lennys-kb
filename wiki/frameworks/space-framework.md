---
framework: SPACE Framework
created_by: Nicole Forsgren
guests: [nicole-forsgren]
date_added: 2026-04-08
---

# SPACE Framework

> A five-dimension framework for understanding developer experience that avoids prescribing specific metrics — giving teams flexibility to measure what matters in their context.

## Overview

The SPACE framework was developed by Nicole Forsgren and colleagues as a complement to DORA. Where DORA prescribes specific metrics for pipeline performance, SPACE provides a framework — a set of dimensions to consider — without telling you which specific metrics to use. This makes it more adaptable across different team contexts and more durable as development practices evolve.

The core insight: developer experience and productivity are multidimensional. No single metric captures them. Teams that optimize for one dimension (say, activity/lines of code) can appear highly productive while degrading another dimension (satisfaction, flow state).

## Components / Steps

**S — Satisfaction and Well-being**
How satisfied are developers with their work, their tools, and their processes? This is distinct from happiness (which is too broad and affected by life outside work). Satisfaction surveys focused on specific tools and workflows give actionable signal.

**P — Performance**
What are the outcomes of the work? Quality, reliability, and impact on users/business. Are we building the right things, and are they working?

**A — Activity**
Volume metrics: lines of code, number of PRs, number of commits, number of alerts. Useful in context but dangerous as standalone productivity proxies (especially in the AI era where LLMs generate verbose code by default).

**C — Communication and Collaboration**
How do teams and systems communicate? What proportion of work happens through direct human collaboration vs. automated tools? What does the flow of information look like through the organization?

**E — Efficiency and Flow**
Can developers get into flow? How much time does it take to complete work? What is the throughput of the system?

## Application

SPACE is used as a diagnostic lens, not a measurement checklist. When assessing developer experience, run through each dimension:
- Where do we have good data?
- Where are we measuring proxies rather than outcomes?
- Which dimensions are we ignoring entirely?
- Which dimensions are under-served by our current metrics?

Then design specific metrics appropriate for your context.

## SPACE in the AI Era

Nicole Forsgren recommends adding **Trust** as a sixth dimension for AI-era development:
- How much do developers trust the code AI generates?
- Are they reviewing it rigorously or accepting it uncritically?
- What's the reliability and consistency of AI-generated outputs?

This dimension was unnecessary before AI-assisted coding but is now fundamental. LLMs are non-deterministic — developers can't just accept generated code the way they would a compiler result.

SPACE tends to map well to AI development contexts because it's a framework rather than a prescription. The same dimensions apply; the specific metrics change.

## Sources

- [[guests/nicole-forsgren]] — "How to measure AI developer productivity in 2025" (Lenny's Podcast, 2025-10-19)

## See Also

- [[frameworks/dora-metrics]]
- [[concepts/developer-experience]]
- [[concepts/velocity]]
