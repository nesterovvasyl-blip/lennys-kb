---
framework: Complaint-Storms
created_by: Noah Weiss
guests: [noah-weiss]
topics: [product-development, user-research, team-rituals, product-quality]
---

# Complaint-Storms

> A structured team exercise in which product builders systematically catalog everything wrong with a competitor's product — and then their own — in order to regain fresh, critical eyes and generate a prioritized list of high-impact improvements.

## Overview

Complaint-Storms were developed at Slack around late 2019 / early 2020 to solve a specific problem: teams who live in and build Slack every day become too close to the product to see its flaws. A team of power users cannot reliably design for the next million customers who have never touched the software.

The name is deliberately negative: the goal is to find everything wrong, not to celebrate what works. Starting with a competitor's product before turning the lens on your own product is the key psychological unlock — it calibrates the team's critical standards and makes it easier to apply the same severity of criticism to your own work.

Stripe uses a similar process called [[friction-logging]]. Noah notes that Complaint-Storms and Slack's Customer Love Sprints are complementary — the storms generate the list; the sprints clear it.

## Components / Steps

1. **Assemble a cross-functional team** — product, design, engineering; ideally including a senior leader (Stewart Butterfield typically joined at Slack).

2. **Pick a competitor in an adjacent space** — choose a product in the same category or with overlapping customer journeys (e.g., for Slack: other workplace messaging or productivity tools).

3. **Walk the full customer journey on one shared screen** — from the marketing site, through account creation, onboarding, first value, and day-to-day use. One person drives; everyone else calls out issues.

4. **Catalog every friction point** — confusing terminology, unexpected flows, missing information, places where a new user would stop, decisions that require too much cognitive effort. No filtering — quantity of observations matters.

5. **Repeat with your own product** — now apply the same rigor. The prior calibration on the competitor makes it easier to say hard things about your own product.

6. **Prioritize the output into a burndown list** — sort by impact and effort. This becomes the input for a **Customer Love Sprint**: a two-week team sprint focused solely on shipping the highest-priority, lowest-effort improvements (not prototypes — shipped to production). Goal: ship all of them. The sprint creates a change of pace from big-feature work and generates rapid customer delight.

**Calibration benefit**: Beyond the specific insights, the complaint-storm calibrates the whole team on product quality standards — everyone ends up with a shared felt sense of what "frustrating UX" looks like, which improves every future design decision.

## How to Apply

- Run quarterly for user-facing product teams; twice a year for less user-facing teams.
- Use a competitor first to build shared critical standards before looking at your own product.
- Pair with live user research sessions: watch customers use the software in a shared Slack thread where team members react in real time — engineers, designers, PMs, and researchers all together.
- Don't let findings sit in a doc. Convert them directly into sprint work.
- The goal is not to copy competitors but to get calibrated on what "good" looks like and apply that lens internally.

## Sources
- [[noah-weiss]] — "The 10 traits of great PMs, AI, and Slack's approach to product"

## See Also
- [[friction-logging]]
- [[walk-the-store]]
- [[product-development-lifecycle]]
