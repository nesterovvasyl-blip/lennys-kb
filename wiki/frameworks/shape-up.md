---
framework: "Shape Up"
origin: "Jason Fried and Ryan Singer (37signals)"
guests: [jason-fried, ryan-singer]
date_added: 2026-04-08
---

# Shape Up

> A product development methodology built around fixed time "appetites," tiny teams, and the principle that unfinished work dies rather than drags on forever.

## Origin
Developed at 37signals (makers of Basecamp and HEY) by Jason Fried and David Heinemeier Hansson. The full methodology is available as a free book at basecamp.com/shapeup. Shape Up emerged as a rejection of both Agile/Scrum sprints and waterfall planning — a third way that keeps projects small, time-boxed, and human.

## How It Works

### 1. Appetites, Not Estimates
The foundational shift: instead of asking "how long will this take?", ask "how much time are we willing to spend on this?" This is called an **appetite**. If a feature is worth one week, it gets one week. If it's worth six weeks, it gets six weeks. Work expands to fill the time given — so the appetite is the constraint, not an estimate.

### 2. Six-Week Maximum
No project runs longer than six weeks. Most features take far less. This prevents the long-running projects that are the most demoralizing force in software development.

### 3. Two-Person Teams
Every feature is built by exactly two people: one designer and one programmer. No more. No coordination overhead, no meetings with 18 people, no slow decision-making.

### 4. Shaping Before Building
Before a project is handed to a team, senior people "shape" the work: define roughly what it is, identify the key tradeoffs, sketch the solution at the right level of abstraction. The shaped pitch gives the team latitude — they know what to build but not exactly how to build it.

### 5. Hill Charts
Projects are tracked on a metaphorical hill. **Left side of the hill**: still figuring out how to do the work (unknown territory, uphill effort). **Right side of the hill**: pure execution, the hard thinking is done, it's downhill from here. If work is stuck on the left side when time runs out, it dies.

### 6. Work That Doesn't Finish Dies
If a project isn't complete at the end of its appetite, it almost certainly doesn't get more time. This is the system. The only exception: if work is on the downslope (right side of the hill) and needs two more days, that's fine. If it's still on the upslope, it dies. This prevents zombie projects that drag on for months.

### 7. Two-Week Cool Down
After each six-week cycle, teams take a two-week cool down. Not vacation — people work on loose ends, bug fixes, and things they never had time for. Leadership shapes the next cycle's projects. The cool down replenishes focus and prevents the back-to-back sprint burnout pattern.

### 8. Trading Concessions
During a cycle, the team and leadership continuously negotiate tradeoffs as new discoveries emerge. There's no fixed spec — there's a direction and a budget. When reality diverges from the plan, the question is: what can we trade away to still ship something valuable within the appetite?

## When to Use
- Software product teams that want to avoid endless project drag
- Teams exhausted by back-to-back Agile sprints with no breathing room
- Companies where every project estimate is wrong and everything takes twice as long

## How to Adopt Shape Up
Jason's strong recommendation: **don't switch cold turkey**. Pick a low-criticality project and try it there first. You'll be bad at it the first time (like picking up a guitar for the first time). If you try it on something that matters and it fails, you'll burn the method forever. Build the skill on low-stakes work, then bring it to critical work.

## Ryan Singer's Real-World Extensions

Ryan Singer, the primary architect of the Shape Up book, has added several practical refinements after consulting with companies outside 37signals:

**The 9-Box Kickoff Exercise**: At the start of a cycle, the build team draws a grid of nine boxes (or fewer) representing the major implementation scopes. Nine is the upper bound of the 7±2 cognitive limit — if everything can't fit in nine boxes, the scope is probably too large. This also creates coaching moments between senior and junior engineers.

**Framing before shaping**: Upstream of the shaping session is a "framing" step — narrowing the problem to something specific and concrete. "Calendar" is not a frame. "Customers can't see empty spaces in their schedule" is. Good framing makes shaping fast.

**The shaping session format**: A shaping session brings together a product person, a designer, and a senior technical person (not just any engineer — someone who knows the codebase). Sessions run 3+ hours, working in real time at a whiteboard, trying and breaking ideas. Total time to shape a project: 2–3 sessions if the technology is familiar.

**The dominant failure mode**: The most common Shape Up failure is doing the six-week cycle without real shaping — the build team gets a PRD or Figma file and is told to "vary scope." This predictably fails. Shaping is the load-bearing element; the cycle length is secondary.

**Basecamp is unusually well-suited**: Most companies can't replicate 37signals' conditions: designers who code, no sales team competing for engineering time, and founders in the room for problem definition up until 2021. Teams adopting Shape Up need to find equivalent conditions, not just copy the rituals.

**Where the PM role shifts**: Under Shape Up, the PM moves upstream from sprint shepherding to deep problem framing — understanding the business context, narrowing problems with Jobs-to-be-Done research, negotiating what's really worth six weeks.

## Related
- [[guests/jason-fried]] — co-creator of the framework
- [[guests/ryan-singer]] — primary author of the Shape Up book and real-world extensions
- [[concepts/jobs-to-be-done]] — upstream research Ryan Singer recommends for framing
- [[concepts/velocity]] — what Shape Up is trying to restore

## Sources
- [[guests/jason-fried]] — "Jason Fried challenges your thinking on fundraising, goals, growth, and more" (Lenny's Podcast, 2023-12-17)
- [[guests/ryan-singer]] — "A better way to plan, build, and ship products | Ryan Singer (creator of Shape Up)" (Lenny's Podcast, 2025-03-30)
