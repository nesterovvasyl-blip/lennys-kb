---
concept: Engineering Strategy
guests: [will-larson]
topics: [engineering-leadership, strategy, decision-making, leadership]
---

# Engineering Strategy

## Definition
An engineering strategy is a written articulation of how an engineering organization will make decisions about technology, tooling, team structure, and investment priorities — grounded in an honest diagnosis of the current situation and translated into specific constraints or guiding policies that engineers can apply to real choices. The core insight from Will Larson: every company always has an engineering strategy; it's just often unwritten, which makes it impossible to debug, apply consistently, or improve.

## Guest Perspectives

### Will Larson (via [[will-larson]])
Larson is the most prominent advocate for explicit engineering strategy. His core arguments:

**All companies have a strategy — the question is whether it's written.** When engineers complain there's no strategy, there is one — it's just implicit in decisions already being made. Writing it down is prerequisite to improving it. An unwritten strategy can't be applied consistently across reporting chains, and it's impossible to diagnose whether a PM is misapplying the strategy or the strategy itself is wrong.

**Good engineering strategy is often boring.** The most effective strategies are simple constraints:
- *Carta*: We use only the tools in our standard kit (Eric Vogel's "standard kit" document)
- *Stripe*: We run a Ruby monolith
- *Uber*: We run everything in our own data centers (no cloud)

These strategies made engineers frustrated, but they focused engineering energy on the problems that mattered to the business rather than on building/maintaining diverse tooling ecosystems.

**Strategy as constraint-solving.** The purpose of strategy is to tell people how to invest limited capacity into the problems the company actually cares about. Bad strategy typically stems from a bad diagnosis — usually from wishful thinking about what constraints are real. The diagnosis is the hardest part to get right.

**The Rumelt framework** (see [[good-strategy-kernel]]):
1. Diagnosis: What is actually true about your current situation?
2. Guiding Policy: Given that diagnosis, what stance will you take?
3. Coherent Actions: What will you actually do to implement that stance?

Engineering strategies that have no "actions" tier are inert strategies — everyone nods, nothing changes.

**Write it, then it can improve.** Even a mediocre written strategy is more useful than an excellent unwritten one. You can refine the written one. You cannot refine the phantom one.

## Key Insights
- An unwritten strategy means different layers of the organization are applying different (invisible) versions of it — leading to inconsistent decisions that look like bad judgment but are actually just misalignment.
- The most common failure mode for engineering strategy is a bad diagnosis driven by wishful thinking about constraints. Leaders who believe they can do all the projects at once will write bad strategies.
- Good engineering strategies often constrain choices in ways engineers dislike. The frustration is usually a sign the strategy is doing its job.
- "First rule of strategy: if you write it down, you can improve it." — Will Larson

## Related Pages
- [[will-larson]]
- [[good-strategy-kernel]]
- [[dora-space-frameworks]]
- [[systems-thinking]]
