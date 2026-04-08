---
guest: Tanguy Crusson
role: Head of Jira Product Discovery, Atlassian
episode: "Hard-won lessons building 0 to 1 inside Atlassian | Tanguy Crusson (Head of Jira Product Discovery)"
date: 2024-06-16
topics: [zero-to-one, innovation, incubation, corporate-innovation, product-leadership, atlassian]
---

# Tanguy Crusson

> Tanguy Crusson is the product lead for Jira Product Discovery at Atlassian, a world-class freediver, and one of the most candid voices on the real challenges of building zero-to-one products inside large companies.

## Content

Tanguy has been at Atlassian for over 10 years, with a 50/50 track record on big bets — which he argues is not bad given the base rates. He worked on: the Atlassian cloud developer ecosystem, HipChat, Stride (the successor to HipChat), a failed IT operations business case, the Statuspage acquisition integration, and finally Jira Product Discovery (JPD), launched as generally available in 2023 and now one of Atlassian's fastest-growing products. The episode is a rare, unvarnished look at what corporate innovation actually looks and feels like.

### Why Zero-to-One Is Hard Inside Large Companies

Despite Atlassian's massive advantages (300,000 customers, distribution, resources, flat decision-making, brand credibility), new bets still fail constantly. The core problems:

1. **Misaligned success metrics**: Monthly active users as a universal KPI is wrong for early bets. You want small, targeted cohorts to have great experiences — not maximum raw usage that churns.
2. **The company's tendency to over-invest**: Well-meaning teams offer help that comes with strings — architecture reviews, process compliance, platform integration. These slow you down before you know if the thing has legs.
3. **High bar for "success"**: At Atlassian's scale, a $100M business is a good start, not a home run. This creates pressure to skip early validation.
4. **Loss of startup hunger**: Startups benefit from starvation. Large companies need to artificially create scarcity and urgency.

### Lessons from HipChat's Failure

HipChat was acquired by Atlassian, was "Slack before Slack," and was ultimately sold to Slack (later folded into Salesforce). Three key post-mortem lessons:

1. **Don't eat your own bullshit**: Atlassian's bottom-up adoption playbook worked for developer tools but didn't apply to communication. They assumed it would without validating it. When business teams preferred Slack, Atlassian's traction stayed in tech teams — a fragmented, non-dominant position.

2. **Competitive myopia**: As Slack surged, the HipChat team fell into feature-following mode — reacting to Slack announcements rather than their own customer insights. "Your competitor's roadmap is the manifestation of decisions they made a year ago based on their customer understanding. Following it means you're always behind."

3. **Don't rewrite and platformize simultaneously**: The HipChat rewrite was coupled with building Atlassian's new microservices platform. You can't rebuild the plane mid-flight and also switch plane models. For an established product, this is compounded: you have customers with expectations who will churn while you're unavailable.

### Lessons from Statuspage Integration

Statuspage succeeded eventually (the stock went UP when Atlassian sold HipChat, then the business grew significantly). Tanguy's personal experience was the painful early integration:

- **Startups entering large companies face culture shock**: Loss of decision autonomy, new HR/engineering/design hierarchies, long-term roadmap demands from a company used to 3-year plans when startups think in 3-month sprints.
- **"We bought you" and "we hired you" mean different things**: The message from leadership is "keep doing what you're doing," while the operational reality is dozens of processes and teams that interrupt the startup's daily work.
- **His ideal for future acquisitions**: Tech-in / acqui-hire model — shut down the product, rebuild on Atlassian's platform, and treat the acquisition as accelerating your roadmap by 12 months (which pays back the acquisition cost at Atlassian's scale).

### The IT Operations Business Case That Went Nowhere

Tanguy spent months pitching an IT operations product (which eventually became Jira Service Management under a different team). Everyone was excited, no one said yes or no. His learning: **no one killed it because they agreed it was good; no one funded it because the "why now" was missing.** Large companies have many valid opportunities sitting on shelves. The differentiator is the trigger for urgency. He later watched another team successfully pitch the same concept with a strong "why now."

### Point A: Atlassian's Internal Incubator

Atlassian built an incubation program called Point A, which gave JPD and a handful of other products their structure. The program defined four stages:

- **Wonder**: Prove there's a problem area worth pursuing. Articulate why Atlassian should play here and why now. Do this with real data.
- **Explore**: Validate solution concepts with customers. Use Figma prototypes and Zoom sessions — don't write code yet. Get customers to play back whether your solutions would address their problems.
- **Make**: Build in stages: alpha, beta, GA. Use the Lighthouse Users Program.
- **Impact**: Product is live; monitor business impact and integrate with the Atlassian platform.

Stage gates are evaluated with founders and business line heads in a meeting (6-pager read silently, then Q&A). Teams can be sent back — JPD was sent back once before alpha-to-beta. This visibility protects the bets while maintaining accountability.

### Key Tactics for Surviving the Ugly Baby Phase

The "ugly baby phase" — the period where the idea is too early to show results but needs protection from organizational skepticism. Tanguy's toolkit:

1. **Frame failure as the most likely outcome**: Telling the org "this might not exist in six months" paradoxically creates protection. Other teams have less urgency to impose their processes on something that may die. It also creates internal startup mentality.

2. **Weekly internal comms**: Use whatever internal tool is available (Atlassian used Atlas, with project update subscriptions). Post weekly: demos, quantitative progress, and — crucially — **3-minute video snippets from customer conversations** rather than research reports. People watch short videos; nobody reads 30-page research reports.

3. **Show velocity**: Save features to demo every week. "No one wants to fuck with a high-speed train." Momentum is visible even without outcome metrics.

4. **Silo ruthlessly**: Work in a way that keeps the rest of the org away. In Tanguy's case, no engineering manager + contractors = freedom from many Atlassian engineering processes. Being in France (time-zone mismatch) actually helped; fewer people engaged to stop him.

### The Lighthouse Users Program

A structured approach to early customer development that avoids two failure modes: (1) rushing to maximize user numbers before the product is ready, causing churn that's hard to recover from, and (2) hiding behind aggregate research (CSAT, NPS) instead of direct customer relationships.

Stages:
- **10 users**: Intensive co-development. Work in shared Slack channels. Weekly calls. Build specifically for them. Use them as proxies for the broader market — document explicitly why they represent your target customer.
- **10 → 100**: Expand while still doing hands-on onboarding. Test solution variations across different customer profiles.
- **100 → 1,000**: Solve for self-service. This is the graduation gate before general availability.

The team-facing benefit: engineers who know 10 customers by name become product engineers. They push back in planning meetings with "Wait — Maria struggles with X, let's fix that instead." Direct empathy drives better product decisions than any dashboard.

JPD was dogfooding within 2 months. First lighthouse user at month 5. Stayed in alpha ~6 months. Beta lasted ~1 year before GA.

### The Incubate-Iterate-Integrate Pattern

From Noah Weiss (former Foursquare CPO): innovate on the edge of an existing product, iterate until it's right, then integrate back into the core. Examples: Instagram's "Popular" tab (edge experiment) → Explore tab → algorithmic main feed. Tanguy applied this to JPD within Jira: built JPD as a mostly separate UX inside the Jira platform, preserving Jira's existing customers while validating the new experience. Now integrating back.

### Actionable Advice
- When pitching a new idea internally, the "why now" is as important as the "why this."
- Treat acquisitions like hiring: factor integration culture shock into plans, not just revenue and roadmap synergies.
- Resist competitive myopia: use competitor launches as a trigger to re-watch recent customer interviews, not as a feature shopping list.
- In incubation mode, publish weekly — demos, metrics, customer video snippets — rather than waiting for a big readout.
- Work with 10 named customers you know deeply before exposing to thousands.

### Notable Quotes
> "Don't eat your own bullshit." (on assuming past playbooks will work in new markets)

> "Startups have the benefit of starving, and so you need to create scarcity."

> "Be very clear about what we're testing, doing that with data, doing that with personal customer stories. No one wants to fuck with a high-speed train."

> "Keep it about the work." (life motto, paraphrasing Obama)

## Sources
- [[tanguy-crusson]] — "Hard-won lessons building 0 to 1 inside Atlassian | Tanguy Crusson (Head of Jira Product Discovery)"

## See Also
- [[lighthouse-users-program]]
- [[wonder-explore-make-impact]]
- [[product-market-fit]]
- [[tar-pit-ideas]]
- [[compound-startup]]
