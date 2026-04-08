---
framework: R&D to Product Transition
created_by: Ryan J. Salva
guests: [ryan-j-salva]
topics: [big-company-innovation, product-development, incubation, team-structure]
---

# R&D to Product Transition

> A structured approach to graduating an experimental project from a research team to an operational product team inside a large company — preserving innovation momentum while building the operational rigor the product requires.

## Overview

Ryan J. Salva developed this approach while leading the transition of GitHub Copilot from the GitHub Next R&D team (which incubated it) to a full EPD (Engineering, Product, Design) product team. The challenge: how do you move a cutting-edge research project into production without killing the magic, losing institutional knowledge, or burning out the researchers?

## Components / Steps

**1. Establish the R&D team structure**
Ring-fence a dedicated team whose explicit job is horizon-two/three work. This team is exempt from normal product requirements: security audits, accessibility compliance, uptime SLAs, etc. They need space to create and experiment without the overhead of production systems.

**2. Identify the graduation signal**
Don't graduate on a calendar. Graduate when three things align:
- A representative customer set with a genuine problem
- Medium-confidence signal that the solution is actually working ("magical" feedback)
- Evidence that the problem-solution fit is real and not just researcher enthusiasm

For Copilot, this was the "mind-blown emoji tweets" and Hacker News threads during technical preview.

**3. Temporarily bridge researchers into the EPD squad**
Move a subset of researchers — not all — into a new EPD squad for a finite period. Their role is knowledge transfer: they carry the vision and technical context that no one else has. They should *not* become permanent product team members.

**4. Staff up behind the researchers**
While researchers are bridged in, hire the permanent EPD talent who will carry the product forward. Researcher departure criteria: replacement is in seat and has absorbed the domain knowledge. This is not a calendar decision.

**5. Transfer full roadmap ownership to EPD**
As soon as the product team has enough context to make good decisions, roadmap ownership must transfer completely. The R&D team should not retain influence over the product roadmap — the team closest to customers must own this.

**6. Return researchers to R&D**
Once the EPD team is self-sufficient, researchers return to the R&D team to work on the next horizon-three project. This cycle preserves the R&D team's culture and prevents researchers from being "consumed" by product work.

## Resource Allocation

Salva's rule of thumb for portfolio allocation at large product teams:
- **5–10%** of capacity: bold experimental research (horizon 2/3)
- **~25–30%**: operations — keeping in-market products meeting expectations
- **~60%**: incremental improvement of existing products

At startups, this collapses to nearly 100% on the single big bet.

## How to Apply
- The R&D team needs air cover from leadership to operate outside normal process constraints
- Engineering fundamentals (SLAs, security, scalability) feel unnatural to researchers — expect resistance and plan for cultural change management
- Give the permanent EPD team full roadmap ownership before the researchers leave; do not let researchers "take the roadmap with them"
- The product team needs to trust that they control their own future, or they will be permanently in the shadow of the R&D team

## Sources
- [[ryan-j-salva]] — "The role of AI in new product development" (2022-09-04)

## See Also
- [[three-inflection-points]]
- [[product-development-lifecycle]]
- [[minimum-viable-process]]
