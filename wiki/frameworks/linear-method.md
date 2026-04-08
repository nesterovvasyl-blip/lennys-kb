---
author: karri-saarinen
guests: [karri-saarinen, nan-yu]
---

# Linear Method

> Linear's distinctive approach to software development: cycles (not sprints), one PM, project-lead ownership, opinionated defaults, and no per-feature metrics goals — optimizing for trust, retention, and craft over short-term conversion metrics.

## Content

Karri Saarinen (co-founder and CEO of Linear) describes a coherent set of practices that differentiate how Linear builds product from the norm. Together these practices form what they call the "Linear Method" — an opinionated philosophy about how software teams should work.

### Cycles, Not Sprints

Linear uses "cycles" instead of sprints. The name is intentional: "we're not sprinting anywhere." Cycles auto-schedule work, protecting teams from infinite backlog distraction. The key function: when something urgent displaces planned work mid-cycle, there's a defensible answer for why original items weren't completed — and a mechanism for resetting scope without losing accountability.

### One PM Model

At ~50 people, Linear has one PM (head of product). Each project instead has a "project lead" — an engineer or designer who is responsible for shipping, communicating, and figuring out scope. This is not a formal role, just an assignment per project. The philosophy: having a dedicated PM for every project creates comfortable specialization where engineers stop thinking about product. Removing the PM layer forces every builder to take ownership of the user experience, not just their technical component.

### Ship Ugly Internally, Polish for Everyone

Linear ships features to internal staging within the first week of development — before designs are finalized. Then they find 1-5 willing customers to co-create with in an early access state where "things can be a little janky." Only at general release does the full quality bar apply. This resolves the tension between perfection paralysis (waiting until things are perfect before getting feedback) and shipping garbage to users.

### No Metrics-Based Feature Goals

Linear doesn't set metrics targets for individual features. Instead, they pair qualitative judgment (does this solve the problem? do customers confirm?) with selective data review (what is the current state?). The rationale: "data didn't make that choice for us." Linear is in the trust and retention business — users commit to Linear long-term — so optimizing for any single metric can damage the relationship that drives long-term success.

### Opinionated Defaults

Linear makes strong choices about how software development should work, rather than offering infinite configurability. This reduces cognitive load for users, creates shared vocabulary and workflow across teams, and signals deep understanding of the problem. See [[opinionated-defaults]] for the full concept.

### Main Quest vs. Side Quests

Karri uses an RPG metaphor for focus: the company has main quest lines (build great product for customers) and side quests (T-shirts, social media, new partnerships). When evaluating any new request, ask: "Is this important for the main quest line now, or is it a side quest?" He applied this principle to himself — delaying podcast appearances until Linear had enough scale to make the conversation interesting.

### Results

Linear has been profitable for two years running with a "net negative lifetime burn rate" — more cash than they've ever raised. Used by Block, Vercel, Ramp, Retool, Mercury, and thousands of startups.

### Nan Yu's Additions

Head of Product Nan Yu adds several operational details to the Linear Method:

**The 10% rule for speed**: By the time 10% of a feature's time budget has elapsed, there should be something workable that tests the core hypothesis. Not polished, not complete — but real enough to validate direction. This surfaces wrong assumptions before 80% of resources are committed.

**Extreme version testing for creativity**: When facing a design decision, build the most extreme version along each key attribute (most safe, most fast, most flexible, etc.). Actually ship those extremes to small internal/beta audiences. Learn what the extremes feel like before converging on the balanced answer. The draft-saving feature is the case study: Linear built the most unsafe version (instant delete, no autosave) and the most safe version (autosave every keystroke), learned from both, then found the nuanced middle.

**The double triangle for PM role**: PM sits between two triangles — (1) PM + engineering + design (building), and (2) PM + sales + marketing (selling). PMs know the customer's native language better than anyone; this knowledge should actively inform marketing language and sales strategy, not just product decisions. Linear embeds a product marketer within the PM team.

**IC-first product decisions**: When evaluating feature requests from enterprise buyers, the hard rule is: if it makes ICs' daily workflows worse to provide reporting for middle managers, the answer is no. Customization features that serve managerial reporting at the cost of IC experience are categorically rejected — this is the most important line Linear holds.

## Sources

- [[karri-saarinen]] — "Inside Linear: Building with taste, craft, and focus" (2023-10-08)
- [[nan-yu]] — "Linear's secret to building beloved B2B products" (2025-01-30)

## See Also

- [[opinionated-defaults]]
- [[friction-logging]]
- [[taste-as-competitive-advantage]]
- [[product-craft]]
