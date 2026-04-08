---
framework: Product Strategy Stack
created_by: Ravi Mehta
guests: [ravi-mehta]
date_added: 2026-04-08
---

# Product Strategy Stack

> A five-level hierarchy that separates mission, strategy, product strategy, roadmap, and goals into clearly defined layers — enabling both top-down strategy building and bottom-up strategy debugging.

## Overview

Developed by Ravi Mehta at Tripadvisor and later formalized in his Reforge Product Strategy program, the Product Strategy Stack gives product teams a common language for terms that are routinely conflated. When a PM can't decide between feature A and feature B, Ravi's diagnosis is almost always that one or more levels of the stack aren't clearly defined — especially at the strategy level.

The framework works in two directions: top-down to *build* strategy, bottom-up to *debug* why something isn't working.

## Components / Steps

### Level 1: Company Mission
The change the company wants to bring to the world. Qualitative and aspirational — describes the company's purpose.

Example: Tinder's mission is to "make single life more fun." Hinge's mission is to be "designed to be deleted."

These are fundamentally different missions that drive every downstream decision.

### Level 2: Company Strategy
The rigorously logical plan the company will use to achieve the mission. Specific, not aspirational. "How we're going to get there."

Ravi treats strategy and vision as potentially combined: a single statement can describe both the vision of the future and the role the company plays in getting there.

### Level 3: Product Strategy
The connective tissue between company strategy and product team decisions. Answers: what specifically will the product do to advance the company strategy, and how?

This is where product team priorities are set. Without a clear product strategy, roadmap decisions become arbitrary.

Example: Tinder's product strategy emphasizes lightweight, serendipitous interactions (no complex filters) — because the mission is to make single life fun, not to be a search engine for people. Hinge's product strategy emphasizes depth-first profiles (prongs, prompts) because the mission requires forming lasting impressions leading to relationships.

### Level 4: Product Roadmap
The sequence of specific initiatives derived from product strategy. What will actually be built, and in what order.

The roadmap should visually include wireframes — not just text descriptions — because visual representations force specificity and reveal trade-offs that words obscure. (Ravi calls this the "blueprint" principle, borrowed from architecture.)

### Level 5: Product Goals
Measurable outcomes tied to the roadmap. Goals are *last*, not first, because they only make sense in the context of a defined destination.

Ravi's road trip analogy: decide you're going to Vegas (mission + strategy), design the route (product strategy + roadmap), and *then* "250 miles" is the meaningful measure. Goals first = "drive 250 miles" with no destination.

## Application

**Building top-down**: Start at mission, work down. Each level should logically derive from the level above.

**Debugging bottom-up**:
- Goals not being hit → check if roadmap items actually support them
- Roadmap not making sense → check if product strategy is clearly articulated
- Product strategy unclear → check if team understands company strategy
- Company strategy unclear → go back to mission

**Wireframes in strategy docs**: When writing a product strategy document, include wireframes of what the product looks like when the strategy is implemented. If you can't agree on the 4-5 nav items of a mobile app after reading the strategy doc, the strategy isn't specific enough.

**Common failure mode**: Starting with goals ("increase retention by 20%") and working backwards. This optimizes for metric movement without strategic coherence, and produces roadmaps that look busy but don't build toward anything.

## Sources

- [[guests/ravi-mehta]] — "How to build your product strategy stack | Ravi Mehta (Tinder, Facebook, Tripadvisor, Outpace)"
