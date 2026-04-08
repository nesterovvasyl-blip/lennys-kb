---
guest: Nan Yu
role: Head of Product at Linear
episode: "Linear's secret to building beloved B2B products | Nan Yu (Head of Product)"
date: 2025-01-30
topics: [product-management, b2b-saas, product-development, customer-research, hiring, speed-and-quality, go-to-market, linear-method]
---

# Nan Yu

> Head of Product at Linear who reveals the operating philosophy behind one of the most beloved B2B SaaS products ever built: speed and quality are not a trade-off, and the best solutions always feel obvious in hindsight.

## Bio

Nan Yu is Head of Product at Linear, the project management tool that has become the gold standard for high-performing engineering teams. Before Linear, Nan worked in product at Mode Analytics (a BI tool) and Everlane (direct-to-consumer fashion). His background spans highly competitive tool categories — places where distinguishing yourself requires seeing from angles others miss. Linear is the #1 tool people wish they could switch to when surveyed about their B2B SaaS stack; the number-one dream switch is from Jira to Linear.

## Key Ideas

### Speed and Quality Are Not a Trade-Off

The dominant narrative is that teams choose between moving fast and building well. Nan's view: this is a false trade-off believed by slow people. When you watch experts — Magnus Carlsen at speed chess, a master chef, a top programmer — you can predict the quality of their output by how fast they move. Speed is a signal of competence, not sloppiness.

What speed actually means at Linear: by the time 10% of the allotted project time has elapsed, you have something workable that tests the core hypothesis internally. Not a polished prototype — a working thing. This surfaces incorrect assumptions before you've sunk 80% of your resources. The first version is never expected to be great; the expectation is that it validates or invalidates the major assumptions quickly.

Patrick Collison captured it: "Good, cheap, fast — choose two" is misinformation spread by the slow. Slow and expensive usually go together.

### The Circle of Release

Linear uses a gradually expanding circle of users for every feature. First circle: internal users (everyone at Linear uses Linear every day — a key advantage). Once it survives internal use without corrupting data or looking broken, release to a beta customer group as early as possible. If no one engages with an early beta, that's a strong signal you missed the mark — before you've invested in polish. Then grow the beta audience, then GA.

### Never Compromise the IC Experience for Middle Management

The most important decision Linear has made: categorically refuse to build customization features that make IC workflows worse in order to make reporting easier for middle managers. Every time a product goes down this path, ICs disengage — they don't fill in fields they don't understand, the data becomes meaningless, and the tool fails everyone.

When buyers ask for these features, Linear's job is to convince them it's a false trade-off. Buyers buy Linear because they want their teams to work more effectively. Features that make ICs disengage undermine the entire value proposition.

The nuance: Linear does build enterprise infrastructure (SAML, SCIM, security controls). What it won't build is anything that makes the day-to-day IC experience worse for reporting purposes.

### Get to the Emotion, Not Just the Goal

Nan's approach to customer research: standard "5 whys" and jobs-to-be-done frameworks are good but can miss the emotional hook. His goal is "to feel bad in the same way that customers feel bad." When he's on sales calls, he keeps asking until he finds the moment the customer actually felt bad — the December 30th ship date that caused a crisis with the marketing team, the tickets thrown over the wall that disappear.

Once you know the emotion someone is trying to avoid, you can build something that eliminates that emotional state. Linear's date flexibility feature (specify Q4, not December 30th) came from someone feeling bad about false precision causing miscommunication.

This is connected to what Paul Graham calls "schlep blindness" — people are so used to the friction in their lives they don't notice it. As an outsider, you can see the spots where improvement is possible.

### Extreme Version Testing for Creative Problem-Solving

When generating options, Linear asks: what's the most extreme version of this along some key attribute? Not as a thought experiment — they actually build and test the extreme versions. Draft saving example: they built the most unsafe version (no auto-save, instant delete), confirmed it felt unsafe, then built the most safe version (auto-save everything on first keystroke), confirmed it left a mess of untitled drafts. The right answer emerged from having genuinely felt both extremes.

This process expands the search space. Most teams only see three options, none of which are right. The fourth option — the correct one — is often in a corner they never looked in.

### The Double Triangle: PM as Bridge Between Building and Selling

The typical PM collaboration model is a triad: PM + engineering + design. Nan argues the second, equally important triad is PM + sales + marketing. PMs understand the customer's native language at a depth no one else in the company does. That understanding should inform the exact words on the website, in release notes, in email campaigns.

At Linear, the PM team includes a full-time product marketer. Her job: make sure all release notes and campaign language are native to the language engineers and PMs actually speak — avoiding the "stink eye" from expert practitioners who immediately detect inauthenticity. Sales validates this language in the field.

This is the opportunity most PMs leave on the table: they're already doing great work with engineering and design, but not yet maximizing impact through go-to-market.

### Deadlines: Use Them Rarely, But Mean Them

Having too many deadlines devalues all of them. When Linear commits to a deadline — usually tied to a marketing launch — it becomes a P0. No one gets pulled off it. As PM, the job is to cut scope until something real and shippable exists at the deadline. The goal: reach a state where you have an actual choice to say yes or no to shipping, rather than "it's not even close to done."

Marketing launch opportunities are scarce — 12 months, 4 quarters, 52 weeks. Missing a window isn't free; you don't get it back.

## Frameworks

### Kneeling (Feature-Reality Fit)

When a feature goes out and feedback comes back, the question isn't "how many people complained?" It's "did we think about this correctly?" If a piece of feedback reveals a conceptual mismatch with reality, a small number of data points is sufficient to act. Volume matters for general popularity signals; quality of insight matters for design correctness.

### Accumulating Opportunity Understanding

Linear maintains a backlog of ~20–30 product opportunities that aren't ready to build yet. For each one, they accumulate understanding over time — new customer conversations, usage patterns, design hypotheses. The question isn't just "do we have a solution?" it's "how much of the problem should we actually take on?" Taking on too much overpromises; taking on too little leaves the real problem unsolved.

## Key Quotes

> "My goal is to feel bad in the same way that customers feel bad." — Nan Yu

> "If you look at people who are at the pinnacle of their craft, you can basically tell how good the output is going to be of their work product by how fast they're going." — Nan Yu

> "The stuff that we absolutely have to say no to is the exact kind of thing that leads to this bloatedness that makes ICs hate their lives." — Nan Yu

> "The best solutions are always obvious in hindsight, and it's just like you have to develop a process internally to eventually find your way there." — Nan Yu

> "When you adopt a tool, you're not just adopting the actual software — you're adopting the idea that this is a practice you ought to be doing in the first place." — Nan Yu

## Actionable Advice

- When starting a project, have a working testable version by the time 10% of your time budget has elapsed.
- Map your customer's emotional journey, not just their goals. Ask questions until you find the moment they actually felt bad — that's what to solve.
- When debating a product decision, ask: what's the most extreme version we could build along each key dimension? Then build both extremes fast and learn.
- Get deeply involved in the words your marketing team uses. As a PM, you know the customer's language better than anyone. Don't outsource that.
- To land a PM job: figure out what burning problem the hiring manager needs solved, position yourself as the solution to that specific problem. Act like you already work there.
- When you have a true deadline, treat it as P0. Cut scope ruthlessly until you have something real you can choose to ship or not.

## Related Pages

- [[frameworks/linear-method]]
- [[concepts/product-led-growth]]
- [[concepts/opinionated-defaults]]
- [[concepts/feelings-over-metrics]]
- [[concepts/velocity]]
