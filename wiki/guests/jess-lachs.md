---
guest: Jessica Lachs
role: VP of Analytics and Data Science at DoorDash
episode: "Building a world-class data org | Jessica Lachs (VP of Analytics and Data Science at DoorDash)"
date: 2024-07-14
topics: [data, analytics, metrics, hiring, doordash, team-structure, data-science]
---

# Jessica Lachs

> VP of Analytics and Data Science at DoorDash, architect of one of the largest and most impactful data orgs in tech. Came up through operations and taught herself data science to solve problems that needed solving.

## Content

Jessica Lachs has spent over 10 years at DoorDash, starting as the first GM (launching Boston in 2014) before pivoting into analytics and building what is now a globally respected data organization. She is unusually candid about her non-traditional background — she's self-taught in Python and SQL — and how that shaped her philosophy of what great analytics work looks like.

### Key Ideas

- **Analytics as Business Impact Driver, Not Service Function**: Lachs's defining belief: analytics should have a seat at the table alongside product, engineering, and ops — not exist to answer questions in a Jira ticket queue. "For me, analytics is a business impact driving function, not purely a service function. Not just answering the why, but answering the 'what do we do now that we know this?'"

- **Centralized Org Model (Counter-Conventional)**: Most companies embed analytics within business units. Lachs strongly disagrees. She argues for a centralized analytics org with pods that *map to* business units (so they feel embedded) but report centrally. Benefits:
  1. *Consistent talent bar* — you can enforce the same hiring rubric across all hires
  2. *Career growth pathways* — analysts can move between domains without leaving the team; no dead ends
  3. *Consistent methodologies and metrics* — one definition of "sales," one churn prediction model shared across teams
  4. *Scale-sensing* — you see the same problems appearing across functions and can get ahead of them
  5. *Team culture and brand* — creates a learning community (the "A-Team") that attracts top talent

- **Goals Aligned with Partner Teams**: The key to making centralized work: analytics shares the same goals as the teams it serves. Marketing analytics has the same marketing goals as the marketing team. This prevents the "service org" dynamic — you're incentivized to work on the most important things because they're your goals too.

- **Proxy Metrics for Long-Term Outcomes**: Lachs's core metric philosophy: never goal on the ultimate long-term metric (e.g., retention). Retention is almost impossible to move meaningfully in the short term. Instead, find the short-term inputs that drive long-term outputs, and validate the causal relationship through experimentation. "Find a short-term metric you can measure that drives a long-term output."

- **Keep Metrics Simple**: Data scientists tend to love composite metrics with coefficients. Lachs actively discourages this. If people don't understand the metric intuitively, if they can't tell whether 0.35 is good or bad, the metric is useless. "Even if it's not perfect, a simple metric that people understand will drive better outcomes than a perfect composite score that nobody understands."

- **Track Fail States, Not Just Averages**: DoorDash has a metric called "Never Delivered" — orders that simply don't arrive. It's rare, but each one triggers churn and is very expensive (refund + re-order + extra dasher). By making Never Delivered a dedicated goal with a dedicated team, DoorDash actively hunts down failure modes that would be invisible in aggregate metrics. The insight: averages hide catastrophic edge cases.

- **Common Currency for Trade-offs**: Lachs's team has quantified every lever of DoorDash's business in common terms (GOV — Gross Order Value). If you lower price by $1, what do you get in GOV? If you cut delivery time by 1 minute, what's the GOV impact? This common currency enables cross-functional trade-off decisions: should marketing spend the dollar, or should logistics spend it improving delivery speed?

- **Hackathons for Exploratory Work**: The tension between answering known questions and finding unknown opportunities is real. Lachs protects exploratory time through hackathons — dedicated days where the team goes off-roadmap to investigate interesting signals. The referral fraud discovery (finding that referral had a bimodal distribution hiding massive fraud) came from one of these hackathons. Exploratory work is where the next roadmap comes from.

- **Hiring: Curiosity Is the Non-Teachable Skill**: Technical skills are table stakes. What Lachs looks for that others miss:
  - *Curiosity* — does this person pull on threads even when they could declare the task complete? Does something "a little off" make them dig in?
  - *Seeing beyond role boundaries* — the best analysts call customers, build product specs, and do engineering work when that's what's needed
  - She embeds "intentionally wrong" elements into case interviews to test whether candidates notice, and how they respond to being corrected

- **Non-Traditional Backgrounds as Strength**: Lachs's own background is in finance and operations — she's "a job I'd never be hired for" by traditional standards. But she believes her non-data background makes her better at the job: she hired for the technical skills she lacked, and her finance/business lens kept the team focused on impact rather than technical elegance.

### DoorDash Culture Elements

- **WeDash**: Every employee dashes four times a year, building first-hand empathy with all sides of the marketplace
- **Extreme Ownership**: The culture from Tony Xu — "what does it take to win?" People do whatever is needed regardless of job description
- **TruthSeek**: A company value — actively seek truth, especially disconfirming evidence

### Memorable Quotes

> "For me, analytics is a business impact driving function — not just answering the why, but answering the 'what do we do now that we know this?'"

> "Retention is a terrible thing to goal on. Find the short-term metric that drives the long-term output."

> "Even if it's not perfect, a metric people understand will outperform a perfect composite score nobody can interpret."

> "I have a job I'd never be hired for."

### Frameworks Referenced

- [[experimentation-culture]] — related to DoorDash's test-and-learn approach
- [[retention]] — Lachs's views on proxy metrics vs. retention as a goal

### Related Guests / Concepts

- [[growth]] — metrics and measurement for growth
- [[product-market-fit]] — data-driven PMF detection

## Sources

- *Building a world-class data org | Jessica Lachs (VP of Analytics and Data Science at DoorDash)* — Lenny's Podcast (2024-07-14)
