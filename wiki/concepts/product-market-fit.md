---
aliases: [PMF]
guests: [adam-grenier, adriel-frederick, jag-duggal, ivan-zhao, noah-weiss, rahul-vohra, sean-ellis]
---

# Product-Market Fit

> The alignment between what you're building and what the market needs.

## Content

Product-market fit (PMF) is the foundational condition for sustainable growth: your product solves a real problem for a real, reachable market, and customers demonstrate this through retention, word-of-mouth, and willingness to pay.

**PMF is not static.** Two important perspectives from the knowledge base challenge the idea that PMF is a one-time achievement:

- **Adam Grenier** argues that when economic conditions shift — recession, inflation, a platform change — you should assume you've lost PMF. The customer base has changed fundamentally: their priorities, budgets, and alternatives are different. Products that were well-fitted pre-shift may be misaligned post-shift, even if the product itself hasn't changed.

- **Adriel Frederick** highlights the "crossing the chasm" dynamic: early adopters differ drastically from mainstream users in motivation, tolerance for rough edges, and how they discover products. PMF with early adopters does not automatically transfer to the mainstream. Teams must re-validate fit as they expand to new segments.

**Measuring PMF — the Sean Ellis score:**

**Jag Duggal** describes Nubank's operationalization of the Sean Ellis methodology as the most rigorous PMF measurement system he's encountered. The question: "How disappointed would you be if this product went away?" (very disappointed / somewhat disappointed / not disappointed). The threshold Sean Ellis established: 40% "very disappointed" = PMF. Nubank raises this to 50% for their Brazilian market, adjusted for cultural optimism. Crucially, Nubank uses this score as a *gate before scaling*, not just a post-launch measurement — products that don't hit the threshold are iterated, not scaled regardless of internal pressure.

Duggal's additional technique: when aggregate Sean Ellis scores are mediocre (e.g., 40%), find the *bullseye cohort* — the small segment scoring 60–70%+ — and understand what defines them. The product roadmap then systematically makes the full customer base look more like that cohort.

**PMF as a gradual ramp, not a milestone:**

**Ivan Zhao** (Notion) describes PMF as something that "never hit us as a binary state." After three to four "lost years," the signs that things were working were gradual: revenue starting, investors knocking, cold outreach from investors. The more distinctive signal: when an investor told him he was taking meetings purely for external validation, not because he needed money. Going back to full building mode after that realization marked the real transition. Zhao's lesson: the absence of clear PMF signals doesn't mean the product is worthless — it may mean the form factor is wrong while the underlying vision is right.

**PMF as stacked S-curves:**

**Noah Weiss** (Slack) describes PMF not as a single achievement but as a series of S-curves. You achieve PMF with a small, specific cohort (e.g., tech-savvy small dev teams), hit exponential growth, then plateau as you saturate that cohort. The next phase requires re-achieving PMF with a new segment (e.g., non-technical knowledge workers at large enterprises). Each segment has different needs, different onboarding friction, and different comprehension barriers.

Slack's self-service plateau in 2019 was precisely this: PMF with early adopters did not extend to the mainstream. The fix required abandoning the existing roadmap entirely for six months to re-learn what the next audience needed — discovering that comprehension ("what is this for?"), desirability ("why should I care?"), and free trial of paid features were the new levers. The resulting north star metric — "Successful Teams" (5+ people using Slack the majority of the work week) — predicted 400% higher upgrade likelihood over 6 months and unified the whole product org.

**Sean Ellis's own framing:**

**Sean Ellis** (the creator of the test) describes it explicitly as a **leading indicator**, not a final judgment — retention cohorts are the ground truth. The test's value is speed: you can get a PMF signal on day one without waiting for longitudinal data. Ellis's full methodology:

1. Survey active users (2+ uses, within the past 1-2 weeks; min 30 responses)
2. Dig into the "very disappointed" cohort — run open-ended and multiple-choice benefit surveys
3. Ask "why is that benefit important to you?" — the contextual answer becomes your best acquisition hook
4. Don't obsess on "somewhat disappointed" users unless they share the core benefit of your must-have users (the Superhuman approach)
5. Sequence your growth work: understand must-have value → optimize activation → build engagement/referral → refine revenue → then scale acquisition channels

The canonical activation case study: at LogMeIn, 95% of signups never completed a remote control session. A company-wide feature freeze to focus on this single metric improved signup-to-usage from 5% to 50% in three months, unlocking customer acquisition channels from $10K/month to $1M/month.

**Practical implications:**
- Continuously resurvey customers after major market events
- Treat each new user segment as a separate PMF question
- Watch retention and activation metrics for early signs of fit erosion
- Use the Sean Ellis score as a launch gate, not just measurement; define your threshold based on your specific customer base
- Find the bullseye cohort (highest PMF segment) and design toward them
- Sequence growth work: nail activation before scaling acquisition

**Rahul Vohra's PMF Engine:**

**Rahul Vohra** (Superhuman) built the most systematic operationalization of Sean Ellis's approach. The Superhuman PMF Engine has four counterintuitive steps:

1. Survey: "How would you feel if you could no longer use this product?" — very / somewhat / not disappointed
2. Target 40%+ "very disappointed" (the Sean Ellis benchmark)
3. Ignore feedback from "very disappointed" — they already love it; don't distract your roadmap
4. Focus entirely on "somewhat disappointed" users **whose main benefit resonates** — find the small thing holding them back

Half the roadmap goes to doubling down on what "very disappointed" users love. Half goes to removing top objections from "somewhat disappointed" users who resonate with the core benefit. This creates a guaranteed mathematical path to increasing the score. Rahul still uses it on new product lines (e.g., Superhuman for Sales).

Superhuman ran manual one-on-one onboarding for every user for years — up to 20 people doing it at peak. This created the early cohort of super-fans whose word-of-mouth bootstrapped Superhuman's brand before any marketing investment.

## Sources

- [[adam-grenier]] — "Assume you've lost PMF when economic conditions shift — the customer base has changed fundamentally"
- [[adriel-frederick]] — "Early adopters differ drastically from mainstream users" (crossing the chasm framing)
- [[jag-duggal]] — "Sean Ellis score as a launch gate; bullseye cohort methodology at Nubank"
- [[ivan-zhao]] — "PMF as a gradual ramp; hiding vision behind accessible form factor"
- [[noah-weiss]] — "PMF as stacked S-curves; Slack's self-service plateau and Successful Teams metric"
- [[sean-ellis]] — PMF test creator; sequencing growth from activation first to acquisition last; LogMeIn activation case study

## See Also

- [[wartime-product-management]]
- [[experimentation-culture]]
- [[diversity-product-velocity]]
