---
framework: Superhuman PMF Engine
created_by: Rahul Vohra
guests: [rahul-vohra]
date_added: 2026-04-08
---

# Superhuman PMF Engine

> An algorithmic framework for measuring, diagnosing, and systematically increasing product-market fit — turning PMF from a feeling into a number you can optimize.

## Overview

Developed by Rahul Vohra at Superhuman and published in a First Round Review post ("How Superhuman Built an Engine to Find Product Market Fit"), this framework makes product-market fit measurable and actionable. Rather than guessing whether you have PMF, or treating it as a binary yes/no, the engine gives you a score you can track and a roadmap algorithm that guarantees improving it.

The framework is based on Sean Ellis's benchmark question and Vohra's system for acting on the results in a counterintuitive but powerful way.

## Components / Steps

### 1. Measure PMF with the Sean Ellis Question

Survey all users: "How would you feel if you could no longer use this product?"
- Very Disappointed
- Somewhat Disappointed
- Not Disappointed

**Benchmark**: Companies that struggle to grow almost always have <40% "Very Disappointed." Companies that grow fastest almost always have >40%. This metric is more predictive of growth than NPS.

### 2. Segment Your Respondents Into Three Groups

- **Very Disappointed** (VD): Already love the product. Don't over-optimize for them.
- **Not Disappointed** (ND): Too far from loving it. Essentially a lost cause for PMF purposes — ignore their feedback.
- **Somewhat Disappointed** (SD): They kind of love it, but something is holding them back.

### 3. Find the "Main Benefit" of Your Product

Ask your Very Disappointed users: "Why do you love the product? What is it about my product that you really value?" Identify the one or two things that come up most — this is your *main benefit*. For Superhuman, it was speed and keyboard shortcuts.

### 4. Split the Somewhat Disappointed Group

Among Somewhat Disappointed users, separate:
- **SD who value your main benefit**: These are addressable. Something small is holding them back. Fix that thing and they'll become Very Disappointed.
- **SD who don't value your main benefit**: Building what they want would pull you in the wrong direction. Politely disregard them — they're pulling the product away from what your core users love.

### 5. Find What's Holding Back the Addressable Somewhat Disappointed

Ask this segment: "What's the one thing that would make our product a must-have for you?" These answers tell you what to build next. Typically, something small (a missing feature, a rough edge) is blocking them from full conviction.

### 6. The Roadmap Algorithm

At each planning cycle:
- **Spend half your time doubling down on what Very Disappointed users love** (to increase retention and depth of love in your existing base)
- **Spend half your time removing blockers for the addressable Somewhat Disappointed** (to convert them to Very Disappointed and raise the overall PMF score)

This guarantees monotonic improvement in PMF score over time.

## Application

Run the survey at launch, and repeat at the beginning of each planning cycle. For mature products, run it on specific sub-products or features rather than the whole product.

Consider using email surveys (how Sean Ellis originally benchmarked it) or in-product interstitials — but be consistent in your measurement method, since changing methods invalidates historical comparisons.

For early stage: run the engine on the whole product. Once you have multiple meaningful user segments (enterprise vs. prosumer, Superhuman for Sales vs. core, etc.), run it on each segment separately.

**Key insight**: Getting to >40% "Very Disappointed" doesn't mean making the product great for everyone. It means finding the segment for whom your main benefit is the most important thing, and making it great for that specific segment — then gradually expanding from there.

## Sources

- [[guests/rahul-vohra]] — "Superhuman's secret to success | Rahul Vohra (CEO and founder)"
- Original First Round Review post: "How Superhuman Built an Engine to Find Product Market Fit"
