---
aliases: [product velocity, engineering velocity, shipping speed]
guests: [geoff-charles, farhan-thawar, gaurav-misra, nicole-forsgren, nick-turley]
---

# Velocity

> The rate at which a product team learns and ships — not just how fast they write code, but how quickly they move from idea to customer value to feedback to next iteration.

## Content

Velocity is the most discussed operational concept across multiple Lenny's Podcast episodes, particularly from Ramp (Geoff Charles), Shopify (Farhan Thawar), and Captions (Gaurav Misra). Each guest offers a distinct implementation of the same underlying principle: the team that can iterate fastest wins, because iteration is the mechanism by which you find what works.

### Geoff Charles (Ramp) — Velocity as Organizational Design

At Ramp, velocity is not a cultural value but a design constraint that shapes every decision:

- **Single-threaded teams** with one goal and full shielding from other demands
- **Async status updates** in systems of record; meetings only for collaboration and decisions
- **No bug backlog** — every bug fixed as found
- **Context over control** — VPs give context and constraints, not solutions; teams make the calls
- **Quarterly planning replaced by biannual one-pagers** — less planning, more doing
- Quality and velocity move together, not in opposition: faster iteration cycles mean faster bug discovery and correction

Geoff's definition of velocity: "Not just about moving fast, but about having the conditions that allow continuous learning and improvement."

### Farhan Thawar (Shopify) — Intensity over Hours

Farhan distinguishes between *expanding time* (working longer hours) and *increasing intensity* (getting more done per hour):

- **Pair programming** as the highest-intensity tool: two people on one computer, no multitasking possible, knowledge transfers in real time. Used 4-8 hours/week at Shopify to concentrate effort on the hardest problems.
- **GSD (Get Shit Done) weekly updates**: Every project publishes an update every week, creating a weekly intensity cycle — teams want to show progress.
- **Six-week reviews** with Toby: leadership pairs with teams to unblock problems, not to audit them.
- **Meetingageddon** (annual meeting reset) + async announcement feed reduces IC meeting time to ~3 hours/week.
- **Delete Code Club**: Velocity is also about removing what slows you down. Smaller, cleaner codebases mean faster onboarding, faster debugging, faster feature work.

Farhan's framing: "What if you just did more per minute?" The goal is not longer sprints; it's higher kilojoules per hour.

### Gaurav Misra (Captions) — One Marketable Feature per Engineer per Week

At Captions, velocity is operationalized as a weekly cadence:

- Every engineer ships one marketable feature per week (something a user would come to the app specifically for)
- When time pressure mounts, cut scope — never cut quality
- Ship the minimum that is still useful; user complaints identify what to build next
- Technical debt is strategic leverage: take it intentionally, budget Q4 to pay it back
- Virality signals prioritization: what's resonating on social tells you what people actually want before you build it

Gaurav's heuristic: "If nobody complains after you ship, that's almost a red flag."

### Why Velocity Creates Quality (Not the Opposite)

Multiple guests make the same counter-intuitive point (also validated by Nicole Forsgren's DORA research, cited by Geoff Charles): fast-moving teams produce higher quality, not lower. The mechanism:

1. Tight iteration cycles = fast feedback loops = rapid discovery and correction of issues
2. Short cycle times = less WIP in flight = smaller blast radius when something breaks
3. High-velocity culture = A+ engineers are attracted = higher baseline quality of decisions
4. Lower cost-per-decision = teams willing to revert and try again rather than defending sunk costs

### Common Velocity Killers

Across all three guests:
- Status meetings (all three explicitly kill them)
- Multiple simultaneous priorities per person (violates single-threading)
- Waiting for full specs before starting
- Accumulating technical debt without a payback plan (Gaurav: once you're paying 80-90% interest, you're just keeping the lights on)
- Large batch sizes (Shopify deletes code and rewrites; Ramp ships and iterates)
- Leaders staying in the weeds (blocks the team)

### Nicole Forsgren (Google / DORA) — Velocity in the AI Era

Forsgren warns that measuring velocity as pure speed is insufficient. "We can ship trash faster every single day. We need strategy and really smart decisions to know what to ship." Her reframe: velocity without strategy is not valuable. The bottleneck is usually not engineering speed — it's knowing what to build.

AI accelerates code writing, but not the full development value chain. The strategy work, experimentation design, cross-functional alignment, and quality review are all still rate-limiting. Teams experiencing compounding gains from AI are those who use it to accelerate the full cycle (idea → prototype → A/B test → learning) not just the code-writing step.

Her recommended velocity metric in the AI era: time from idea (or feature concept) to production or customer experiment. This captures the full loop. She also notes that DORA's deployment frequency and lead time are still valid for pipeline health, but must be paired with quality metrics to avoid optimizing for volume.

### Nick Turley (OpenAI / ChatGPT) — Is It Maximally Accelerated?

Turley's culture of urgency at OpenAI is captured in his team's Slack emoji: "Is this maximally accelerated?" It's a forcing function, not a mandate: when someone is working on something, the question asks "if this were the highest priority and we wanted to truly maximize speed, what would we do?" This exposes the critical path versus secondary tasks.

Turley distinguishes velocity in product development (should be very high) from velocity in safety processes (where more process is required). His broader philosophy: learning fast is the core competitive advantage in AI, not just building fast. The only way to know what to polish, what people want, and what the model's real failure modes are is to ship and observe. "You're going to be polishing the wrong things in this space. You won't know what to polish until after you ship."

## Sources
- [[geoff-charles]] — "Velocity over everything: How Ramp became the fastest-growing SaaS startup ever" (Lenny's Podcast, 2023-08-06)
- [[farhan-thawar]] — "How Shopify builds a high-intensity culture" (Lenny's Podcast, 2024-12-19)
- [[gaurav-misra]] — "Inside the expert network training every frontier AI model" (Lenny's Podcast, 2023-02-12)
- [[nicole-forsgren]] — "How to measure AI developer productivity in 2025" (Lenny's Podcast, 2025-10-19)
- [[nick-turley]] — "Inside ChatGPT: The fastest growing product in history" (Lenny's Podcast, 2025-08-09)

## See Also
- [[product-management]]
- [[engineering]]
- [[culture]]
- [[talent-density]]
