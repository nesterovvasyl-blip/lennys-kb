---
framework: Bricklayer to Architect
created_by: Scott Wu
guests: [scott-wu]
topics: [ai-engineering, future-of-software-engineering, autonomous-agents]
---

# Bricklayer to Architect

> AI coding tools shift engineers from doing implementation work (bricklaying) to specifying what should be built and how (architecture) — the highest-value 10% of engineering work.

## Overview

Scott Wu introduced this framework at Cognition to describe how autonomous AI coding agents like Devin transform the nature of software engineering work. The thesis is not that engineers become obsolete — it's that engineers can finally spend the majority of their time doing the part of engineering that actually requires human judgment.

## Components / Steps

**The 10/90 Split (Today)**
Software engineering today:
- ~10%: defining the problem, thinking through architecture, mapping the solution, making key trade-offs
- ~90%: implementation — Kubernetes errors, debugging, migrations, version upgrades, bug reports, testing, documentation

The 10% is the intellectually valuable work. The 90% is what Wu calls the "bricklaying" — necessary but not where unique human value is created.

**The Shift with AI Agents**
Devin and similar autonomous systems automate large portions of the 90%. Engineers increasingly:
- Define the architecture and specify exactly what they want
- Review outputs and provide targeted feedback
- Make the high-leverage calls about trade-offs
- Operate asynchronously across multiple parallel workstreams (each engineer at Cognition runs 4-5 concurrent Devins)

**What "Architecture" Actually Means**
In this framework, architecture is not just system design — it's:
- Precisely defining the problem
- Specifying the solution in enough detail for an agent to execute
- Identifying the key decisions and trade-offs at each step
- Knowing when to intervene mid-execution and what direction to steer

This requires deeper understanding of the system, not less. Wu is emphatic: you still need to be able to "peel back the abstractions" — understand how databases work, what TCP/IP is doing, how the garbage collector behaves. These lower-level concepts inform the quality of architectural decisions.

**The Manager vs. Architect Distinction**
Wu explicitly rejects the framing "manager of Devins" as the right mental model. Management implies emotional overhead, performance reviews, personnel decisions. Architecture implies working at the right level of abstraction to specify, review, and steer. The parallel to Python: when Python abstracted away memory management, programmers didn't become "memory managers" — they became better problem solvers.

## How to Apply

**For individual engineers:**
- Identify the tasks in your current sprint that are pure implementation with clear specs → delegate to Devin
- Start with easy, well-defined tickets to build the agent's knowledge of your codebase
- Invest time in better task scoping — the clearer the specification, the better the output
- Reserve direct code work for the 10-20% where architectural decisions need your judgment

**For engineering teams:**
- Give Devin access to your repo, CI/CD, and testing infrastructure early — this is what lets it verify its own work
- Early adopters on the team should onboard Devin and build its codebase knowledge before rolling out to others
- Think about tasks vs. problems: give Devin specific, verifiable tasks; keep problems with humans

**For learning:**
- Learn to code and understand fundamentals even more deeply than before — the ability to peel back abstractions and specify precisely is more valuable, not less
- Focus on systems thinking: how components interact, what trade-offs matter, how to evaluate approaches

## Sources
- [[scott-wu]] — "Inside Devin: The AI engineer that's set to write 50% of its company's code this year"

## See Also
- [[jevons-paradox-software]]
- [[ai-pair-programmer]]
- [[forward-deployed-engineer]]
- [[context-engineering]]
