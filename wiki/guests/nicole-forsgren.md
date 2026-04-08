---
guest: Nicole Forsgren
role: Senior Director of Developer Intelligence and Core Developer, Google
episode: "How to measure AI developer productivity in 2025 | Nicole Forsgren"
date: 2025-10-19
topics: [developer-experience, engineering-productivity, ai-tools, metrics, devex, dora, space-framework]
---

# Nicole Forsgren

> The researcher who created DORA and SPACE — the most widely used frameworks for measuring developer productivity — and is now rethinking how to measure productivity in the age of AI.

## Bio

Nicole Forsgren created the DORA metrics (Deployment Frequency, Lead Time, MTTR, Change Fail Rate) and the SPACE framework for measuring developer experience. She wrote the foundational book *Accelerate* and co-authored *Frictionless: 7 Steps to Remove Barriers, Unlock Value, and Outpace Your Competition in the Age of AI* (with Abi Noda). She spent time as a researcher at GitHub and Google's DORA team before joining Google as Senior Director of Developer Intelligence and Core Developer. This was her second appearance on Lenny's Podcast (first episode focused on general developer productivity; this episode focuses specifically on AI's impact).

## Key Ideas

### Most Productivity Metrics Are a Lie in the Age of AI

Turley's first provocative thesis: "Most productivity metrics are a lie." Lines of code, long the unspoken proxy for engineering output, is now broken because AI tools generate extremely verbose code by default. "If the goal is more lines of code, I can prompt something to write the longest piece of code ever." The metric is too easy to game and is now measuring AI verbosity, not developer value.

What does still work: DORA metrics, when used precisely for what they were designed — measuring pipeline speed (deployment frequency, lead time) and stability (MTTR, change fail rate). But they can't be blindly applied now because AI has created new feedback loops earlier in the pipeline that weren't previously relevant.

SPACE is more durable because it's a framework, not a prescription. It doesn't tell you which metric to use — it gives you five dimensions to consider: Satisfaction, Performance, Activity, Communication/Collaboration, and Efficiency/Flow. It maps reasonably well onto AI development contexts. Forsgren would add "Trust" as a sixth dimension: how much do you trust the code an AI generates?

### The Trust Problem with AI Code

This is the new frontier challenge: "LLMs are non-deterministic. Right now, we can't just put in a command and get something back and accept it. We really need to evaluate it." Evaluation dimensions: Are we seeing hallucinations? What's the reliability? Does it meet our code style? If it doesn't, is that acceptable?

This evaluation work is a new form of cognitive load for developers. It also means that existing feedback loop structures are too slow — AI is creating feedback loops earlier in the development process that we need to leverage but haven't built infrastructure for yet.

### Flow State in the Age of AI: Interruption and Opportunity

Traditional flow state for developers meant long blocks of focused, uninterrupted code writing. AI changes this fundamentally: you start something, get code back, review it, try to integrate it, and that process interrupts the old flow.

But senior engineers have found a new form of flow: treating themselves as EM (engineering manager) for a set of AI "junior engineers." They prime the AI with architectural requirements, assign pieces to parallel agents, think through hard problems while agents run, and come back to review. This keeps them in a higher-level flow: "What's my goal? What are the pieces I need to get there? How quickly can I get there?"

Forsgren's speculation: AI may make previously useless 45-minute work blocks productive, because the machine can help you re-enter context ("reminding us of context and generating diagrams of the system"). The traditional requirement for 2-hour blocks to achieve flow may relax.

### Developer Experience: Not Just Productivity

DevEx is not synonymous with productivity. It's what it's like to build software day-to-day — friction, workflows, tooling, support. When DevEx is poor, everything else fails. But when it's good, you get a self-reinforcing loop: better work, better flow, better innovation, better products.

The three interlocking dimensions of DevEx: **flow state** (can you get into deep work?), **cognitive load** (how much mental energy is consumed by plumbing rather than problem-solving?), and **feedback loops** (how quickly do you know if what you built works?).

### Start With Listening, Not Tools

The #1 advice for improving developer experience: "Go talk to people and listen." Most teams jump to buying or building tools before they understand the actual friction. Forsgren's example: a company with a slow mainframe process that everyone hated — the fix was just changing from print-and-walk to email. No technology required.

After listening: do surveys. Surveys are faster than instrumentation and give you a landscape quickly. Key survey design: ask people to pick their top 3 friction points (not all of them — that makes data messy), and for each, how often does it affect them (hourly/daily/weekly/quarterly). The frequency weighting creates a meaningful impact score.

Forsgren explicitly does not recommend "happiness surveys" because happiness is influenced by too many life factors. She recommends satisfaction surveys instead: "Are you satisfied with this tool?" is much more tractable than "Are you happy?"

### The Frictionless 7-Step Framework

The book *Frictionless* (co-authored with Abi Noda) provides a seven-step process:
1. **Start the journey**: Listening tour, synthesize findings, visualize workflows
2. **Get a quick win**: Small, visible win to build momentum
3. **Use data to optimize**: Build data foundation, add surveys, use existing instrumentation
4. **Decide strategy and priority**: Use evaluation frameworks to pick what to work on next
5. **Sell your strategy**: Get buy-in, share the plan, get feedback
6. **Drive change at your scale**: Strategies for local (grassroots), global (top-down), and middle-management scope
7. **Evaluate progress and show value**: Measure outcomes, loop back to step 1

A J-curve is normal: quick wins look big early, then a dip as easy wins are exhausted and you build infrastructure, then compounding returns.

### Communicating DevEx Value to Leadership

Frame improvements in terms of what leadership already cares about:
- If they talk about market share → frame in velocity (speed from idea to experiment)
- If they talk about profit margin → frame in cost savings (cloud costs, vendor reduction, recovered headcount time)
- If they talk about transformation/disruption → frame in capability and agility

Don't make them translate. Use their vocabulary. Attribution is complex (was it AI tools or DevEx improvements?), but that's fine — disclose both and show the combined effect.

### Applying a Product Mindset to DevEx

Treat developer experience as a product: identify a problem, find an addressable market (your developers), create MVPs and experiments, measure success, get continuous feedback, sunset things that no longer matter. This is especially important now because with AI, everything is changing rapidly — you need to constantly re-evaluate whether your metrics are still driving the right decisions.

## Frameworks

### DORA Metrics

Four key metrics for measuring software delivery pipeline performance:
- **Speed**: Deployment Frequency and Lead Time (code commit to code deploy)
- **Stability**: MTTR (Mean Time to Recovery) and Change Fail Rate

Still valid for assessing pipeline speed and stability, but must be used in precisely their original scope. Cannot be blindly applied to AI-era development without accounting for new feedback loops.

### SPACE Framework

Five dimensions of developer experience (a framework, not a prescription):
- **Satisfaction**: How satisfied are developers with their work and tools?
- **Performance**: What are the outcomes? (Quality, reliability)
- **Activity**: Volume metrics — PRs, commits, lines of code (useful in context, not as standalone)
- **Communication and Collaboration**: How do teams and systems communicate?
- **Efficiency and Flow**: Can people get into flow? What's the time cost?

In the AI era, Forsgren recommends adding **Trust** as a sixth dimension.

## Key Quotes

> "Most productivity metrics are a lie. If the goal is more lines of code, I can prompt something to write the longest piece of code ever. It's just too easy to game that system." — Nicole Forsgren

> "Most teams can move faster. But faster for what? We can ship trash faster every single day. We need strategy and really smart decisions to know what to ship." — Nicole Forsgren

> "We can't just put in a command and get something back and accept it. We really need to evaluate it." — Nicole Forsgren

> "Happy devs make happy code. They write better programs, they do better work, they're better team members and collaborators." — Nicole Forsgren

> "If you can't answer a question with data, don't get it." — Nicole Forsgren

## Actionable Advice

- Stop using lines of code as a proxy for productivity — it's now measuring AI verbosity, not engineer value
- Use DORA metrics only for what they were designed: pipeline speed and stability
- Start any DevEx improvement effort with a listening tour, not tool purchases
- Survey developers: ask them to pick top 3 friction points and how often they occur, then weight by frequency
- Frame DevEx value in your leadership's vocabulary (market share, margin, velocity, transformation) — don't make them translate
- Bring a product mindset to DevEx: MVPs, experiments, continuous feedback loops, sunsetting old metrics
- Don't run happiness surveys; run satisfaction surveys about specific tools and processes
- Senior engineers should experiment with agentic workflows: prime AI with architecture upfront, assign pieces to agents in parallel, review together

## Related Pages

- [[concepts/velocity]]
- [[concepts/ai-evals]]
- [[frameworks/dora-metrics]]
- [[concepts/developer-experience]]
