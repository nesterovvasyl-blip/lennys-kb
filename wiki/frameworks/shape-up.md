---
framework: "Shape Up"
origin: "Ryan Singer & Jason Fried (37signals)"
guests: [jason-fried, ryan-singer]
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

## Related
- [[jason-fried]] — creator of the framework
- [[constraints-as-advantage]] — the philosophy that small/constrained teams do better work
- [[calm-company]] — the broader 37signals operating philosophy

## Ryan Singer's Additions — Shape Up In Real Life

Ryan Singer codified Shape Up and wrote the book (free at basecamp.com/shapeup). In a 2025 deep-dive episode with Lenny, he added significant nuance around how to apply it outside of Basecamp's unusual structure:

**On shaping sessions:** Three hours is sufficient for a well-framed problem. All three perspectives (product, senior engineer, designer) must be present. The "grumpy old plumber" principle: the engineer should insist on opening the actual code before agreeing to any scope, to surface rabbit holes before the project starts.

**On the 6-week ceiling:** Six weeks is a maximum, not a prescription. Growth teams might run 2-week time boxes. The key is that the ceiling forces you to ask what you can actually finish — not what you'd like to do.

**On shaping output quality:** A well-shaped idea can be described in under 10 moving pieces. The test: can a technical person look at the output and say "I know what to go build"? If not, it needs more shaping.

**The nine-box kickoff exercise:** At project kickoff, the team translates the shaped idea into nine major implementation scopes (9 or fewer). This surfaces scope issues early, creates natural coaching moments for junior engineers, and gives everyone a shared map of the work.

**On when to adopt:** Problems typically become undeniable at 30–50 people in product+engineering. The trigger is often the first project where a founder fully delegates and it goes sideways. Start with a pilot on something meaningful but not critical.

**The dominant failure mode in the real world:** Not enough detail in shaping. Teams regularly get fuzzy handoffs and then fail to ship, blame the method, and revert. The shaping work is where the hard thinking must happen.

## Sources
- Jason Fried — "Jason Fried challenges your thinking on fundraising, goals, growth, and more" (Lenny's Podcast, 2023-12-17)
- [[ryan-singer]] — "A better way to plan, build, and ship products" (2025-03-30)
