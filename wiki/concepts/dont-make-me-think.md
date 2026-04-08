---
title: Don't Make Me Think (Comprehension over Friction)
coined_by: Steve Krug (book); articulated in product context by Stewart Butterfield
guests: [stewart-butterfield]
topics: [product-craft, ux, mental-models, product-design]
---

# Don't Make Me Think

## Overview

Named after Steve Krug's classic UX book, this concept was elevated by [[stewart-butterfield]] as a core design mantra at Slack, arguing that the real goal of product design is to **minimize cognitive load** — not to minimize friction or reduce clicks.

Stewart explicitly pushes back on "reduce friction" as the governing principle, arguing it is the right goal only in a minority of cases, and that **comprehension** is the real challenge most of the time.

## Two Distinct Problems

**Friction problem** (where "reduce friction" is correct):
- The user knows exactly what they want
- The user understands the product
- The obstacle is physical or mechanical (too many form fields, slow load times, broken payment flow)
- Example: buying Taylor Swift concert tickets on Ticketmaster — intent is 100%, comprehension is 100%, friction is the enemy

**Comprehension problem** (where "reduce friction" is wrong):
- The user is at the minimum threshold of interest
- The user doesn't know what the product does or what action to take
- The obstacle is understanding, not mechanics
- Example: a potential Slack user who vaguely heard about it and visited Slack.com — they need to understand what Slack is before any friction is relevant

Stewart's estimate: **70–80% of product design is in the comprehension zone**. Most software surfaces suffer from comprehension problems, not friction problems. Applying friction-reduction thinking to comprehension problems makes them worse.

## The Costs of Making People Think

1. **Metabolic cost**: Decisions require glucose. Neurons fire, ATP is consumed. Decision fatigue is biologically real.
2. **Emotional cost**: If software stops someone and asks them to make a decision they don't understand, they feel **stupid**. Non-technical users especially blame themselves ("I'm dumb") rather than the software. That bad feeling becomes permanently associated with the product.

## The Misapplication of "Fewer Clicks"

A related failure mode: optimizing for number of clicks or taps. Stewart argues this is almost always the wrong metric.

The extreme case: you could make any action in an app a single click by exposing every possible option on one scrolling screen. Obviously terrible. So why do people think a little of this is good?

Stewart's reframe: **if each step requires zero thought, eight steps is fine**. If each step requires a difficult decision, two steps is too many.

His positive example: the original Uber app was "Where would you like to go?" and "Other." Everything else lived under "Other." More options would require more thinking; fewer options made the primary job trivially easy.

## Practical Applications

- **Menu design**: Group related items, show the 2–3 most common actions prominently, put everything else behind "More"
- **Settings and preferences**: Most users never visit them because the options are incomprehensible. Investment in understandable defaults beats investment in more options.
- **New feature discovery**: If users don't understand what a feature does, reducing the number of taps to access it doesn't help
- **Onboarding**: The problem is almost never "too many steps" — it's "don't know what I'm signing up for"

## Connection to Owner's Delusion

[[owners-delusion]] explains *why* comprehension problems are so common: creators design for themselves (high comprehension, high intent) rather than for minimally-aware visitors. Naming both concepts helps teams catch themselves applying the wrong mental model.

## Sources
- [[stewart-butterfield]] — "Mental models for building products people love ft. Stewart Butterfield"

## See Also
- [[owners-delusion]]
- [[utility-curves]]
- [[first-mile-experience]]
- [[taste-as-competitive-advantage]]
