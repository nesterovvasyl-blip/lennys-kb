---
title: Utility Curves
coined_by: Stewart Butterfield
guests: [stewart-butterfield]
topics: [product-craft, prioritization, mental-models]
---

# Utility Curves

## Overview

A mental model popularized by [[stewart-butterfield]] at Slack for understanding whether a product feature or area is worth more investment. It applies a classic S-curve to product development.

## The Framework

Visualize an S-shaped curve where:
- **Horizontal axis**: Cost, effort, or quality invested
- **Vertical axis**: Value, utility, or convenience delivered

The curve has three zones:
1. **First flat section** (bottom): Early investment yields little value. The feature is barely functional, the product barely exists. Think: creating a user table in a database before any product works.
2. **Steep middle section**: Investment translates rapidly into value. This is the critical zone where the product goes from "junk" to "good" to "great."
3. **Second flat section** (top): Diminishing returns. More investment yields marginal improvements.

## The Key Insight

Most features are viewed as binary (you either have them or you don't). The utility curve reveals that both "this feature isn't being used" AND "this feature is maxed out" look like low usage — but they call for opposite responses.

- Low usage on the first flat section → invest more to get up the curve
- Low usage (or stagnant usage) on the second flat section → stop investing here; redirect elsewhere

## The Moving Baseline Problem

Stewart pairs utility curves with Bezos's concept of "divine discontent": customer expectations rise continuously. A feature that was firmly on the "steep middle section" in 2018 may now be on the first flat section because competitor implementations have raised the baseline.

This means even "done" features need periodic re-evaluation. Classic examples: login experiences, password reset flows, checkout flows. These get implemented once and rarely revisited, yet the quality bar has risen considerably.

## Applications

**Feature investment decisions**: Before deprioritizing a feature because it's not performing, ask: are we on the first flat section (not good enough yet) or the second (good enough, time to move on)?

**Product areas**: Apply the same logic to entire product surfaces — is search in the first flat section (needs investment to become actually useful) or the second (search is table stakes and further investment yields diminishing returns)?

**The danger of obsession**: Stewart also warns against the opposite failure — teams that are obsessed with a narrow area and keep investing beyond diminishing returns, past the second flat section. Taste means knowing when to stop as much as when to invest.

## Sources
- [[stewart-butterfield]] — "Mental models for building products people love ft. Stewart Butterfield"

## See Also
- [[taste-as-competitive-advantage]]
- [[owners-delusion]]
- [[dont-make-me-think]]
