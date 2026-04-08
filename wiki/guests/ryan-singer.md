---
guest: Ryan Singer
role: Creator of Shape Up; Product Consultant (formerly Head of Strategy, 37signals)
episode: "A better way to plan, build, and ship products | Ryan Singer (creator of \"Shape Up\")"
date: 2025-03-30
topics: [product-development, shape-up, team-structure, product-process, scrum-alternatives, pm-role]
---

# Ryan Singer

> One of the first hires at 37signals and the creator of the Shape Up methodology, Ryan Singer spent 17 years building Basecamp and codifying a product development approach now adopted by teams worldwide.

## Bio

Ryan Singer joined 37signals (makers of Basecamp) in the early 2000s, working directly with Jason Fried and David Heinemeier Hansson on the first version of Basecamp. He spent nearly two decades as Head of Strategy, and in 2019 published *Shape Up* as a free book at basecamp.com/shapeup. After leaving 37signals in 2021, he began consulting with teams to help them implement the Shape Up methodology in real-world contexts — a journey that revealed how much 37signals' unique circumstances he had taken for granted. He now runs a course called "Shaping in Real Life" specifically designed for teams that don't operate like Basecamp.

## Key Ideas

### The Origin of Shape Up

Shape Up emerged from two constraints at early 37signals: DHH was working only 10 hours per week building the first version of Basecamp, and Jason Fried had an almost obsessive urgency to see forward movement. These two constraints — scarce engineering time and intolerance for fuzzy, open-ended projects — forced an approach where every piece of work had to be crisply defined so that 10 hours of engineering time produced something visibly complete.

The methodology only formalized after the first major project failure — roughly 10 years in — when a team couldn't see the end of a project. That failure revealed that the approach had been spreading organically through culture, but couldn't spread indefinitely by osmosis. Shape Up became explicit at that point.

### The Three Core Elements

**1. Appetites, not estimates.** Instead of asking "how long will this take?" ask "how much time are we willing to spend?" The time is fixed; the scope varies to fit. Six weeks is the maximum because that is roughly the longest horizon over which a team can surface enough unknowns to shape a solution responsibly. Shorter time boxes are fine — growth team work might be one or two weeks.

**2. Shaping.** Before any project is handed to a build team, senior people (product person, designer, and a senior technical person who "knows where the bodies are buried") do a shaping session: a 3-hour-to-a-few-session intensive where they try ideas, break them, and narrow to a clear solution. The output is not a PRD or a Figma file — it's a diagram or sketch from which engineers can say "I know what to go build." Good shaping rule: if the shaped idea can be described in fewer than 10 moving pieces, it's probably clear enough.

The key tool: **breadboarding and fat marker sketching** — communicating just enough about flows and components to convey the idea without locking in implementation details. The right time for Figma is after shaping, during high-fidelity design, not during the shaping session itself.

**3. Team autonomy during the build.** The build team receives the well-shaped idea and creates their own implementation tasks. This is the opposite of Scrum's "paper shredder" — where someone not doing the work creates all the tickets. The team sees the whole idea, understands why it exists, and has freedom to figure out how to make it real. This drives engagement, especially from senior engineers.

### The Dominant Failure Mode: Not Enough Detail

The most common mistake Ryan sees is teams doing Shape Up without real shaping — giving the team a Figma file or a PRD with a calendar entry for a "six-week cycle" and calling it Shape Up. The predictable result: the team has no clarity, keeps asking questions, and fails to ship. Shaping is the crucial ingredient that most teams skip.

The second failure mode: starting the six-week cycle without an engineer in the room during shaping. Without the person who knows the technical terrain, the team will discover hidden complexity mid-cycle — old code branches, unresolved dependencies — that blow up the timeline.

### The 9-Box Kickoff Exercise

A practical tool for teams that aren't all senior: at kickoff, after receiving the shaped pitch, the build team draws a grid with nine boxes (or fewer — the cognitive science principle of 7±2 applies). They fill in the nine major implementation scopes. If they can't fit everything in nine, the scope may be too big. This exercise also creates coaching moments where senior engineers can correct junior approaches before they go wrong.

### When to Try Shape Up (and When Not To)

Shape Up is most useful when founders have stepped back from hands-on work and first delegated to PMs and engineers — roughly when the product+engineering team reaches 30–50 people. At that point, the cultural transmission of urgency and clarity breaks down for the first time.

The largest adoption blocker is organizational sensitivity: CPOs and CTOs don't publicly discuss shipping struggles. Shape Up spreads by word of mouth because teams don't want to be seen as failing.

Shape Up is not a universal transplant. 37signals has properties most companies don't:
- Every designer codes (eliminates the design-engineering wall)
- No sales team (eliminates competing engineering requests)
- DHH managed engineering capacity such that there was reliably clear runway every six weeks
- Founders were in the room for problem definition up until 2021

Teams adopting Shape Up need to find ways to create these conditions, not just copy the rituals.

### The PM Role Under Shape Up

The PM moves upstream. Instead of shepherding the sprint — chasing engineers to see if they're stuck — the PM invests deeply in understanding the business context, narrowing the problem, and doing the framing work. The framing question: "What is really the problem we are solving?" is upstream of shaping, and often requires Jobs-to-be-Done research (Ryan recommends Bob Moesta's *Demand-Side Sales 101* as the practical entry point).

### Basecamp vs. the Real World

Ryan's most important field lesson: teams don't struggle with "feature factory" problems (shipping too much, shipping the wrong thing). They struggle with **projects that won't finish** — dragging projects, teams that can't see the end, endless scope creep. Shape Up primarily solves the finishing problem, not the prioritization problem.

## Frameworks

### The Circuit Breaker

Basecamp's original rule: if a project is not on track to finish at the end of the six-week appetite, cancel it and rethink. Most teams lack the stomach for this. The practical alternative: pull the project out of build mode and back into shaping mode — different people, different questions — to understand what was fuzzy. Don't keep investing in something that isn't working.

### Framing Before Shaping

Before a shaping session, the work is "framing": narrowing the problem to something concrete. "Calendar" is not a frame. "Customers can't see empty spaces in their schedule" is a frame. Good frames make shaping sessions fast and productive; bad frames turn shaping into endless exploration.

## Key Quotes

> "We are not going to start something unless we can see the end from the beginning." — Ryan Singer

> "The dominant failure case I see is always not enough detail. Engineers run back to the product folks saying, 'I'm not getting enough from you.'" — Ryan Singer

> "You can't put 10 pounds of crap in a five pound bag." — (quoting Bob Moesta) Ryan Singer

> "If it's shaped well, you can usually describe it in less than 10 moving pieces." — Ryan Singer

> "The PM moves upstream. They're less busy with 'how do I get this project to not be in a bad state while it's getting built?' and way more in 'how do I understand the business context?'" — Ryan Singer

## Actionable Advice

- Describe any shaped project in 10 or fewer moving pieces; if you can't, it's not shaped yet
- Always include a senior technical person in shaping sessions — someone who knows the technical terrain
- Use fat marker sketches and breadboarding, not Figma, during shaping
- Start Shape Up with a pilot project that is important but not critical to the business
- Match the appetite to the project, not always six weeks — short growth experiments can be one or two weeks
- At project kickoff, have the build team fill in the 9-box grid of major implementation scopes
- If a project is stuck at the end of its time box, return it to shaping — don't extend and don't just cut scope

## Related Pages

- [[frameworks/shape-up]]
- [[concepts/jobs-to-be-done]]
- [[topics/product-development-process]]
- [[topics/pm-role]]
