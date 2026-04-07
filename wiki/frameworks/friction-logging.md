---
author: david-singleton
guests: [david-singleton]
---

# Friction Logging

> A systematic practice for capturing every point of confusion, frustration, or friction encountered while using a product — then using that log to drive prioritization.

## Content

Friction logging is a structured approach used at Stripe, articulated by CTO David Singleton, for maintaining high product quality and catching UX degradation before it compounds. It is a form of deliberate, systematic product empathy that any engineer or PM can practice.

### The Practice

The core mechanic is simple: use your own product end-to-end, and document every moment of friction — confusion, unexpected behavior, slow performance, unclear error messages, missing affordances, or any moment where you had to think harder than you should have. The log is a structured capture of these moments with enough context to act on them.

What makes it "systematic" rather than casual is the discipline of:
1. **Actually doing it regularly**, not just when obvious problems arise
2. **Writing every friction point down** in the moment, not relying on memory
3. **Including context**: what were you trying to accomplish, what did you expect, what happened instead
4. **Prioritizing the log** — friction log items get treated as first-class inputs to product planning, not just complaints

### Why Stripe Uses It

Stripe builds developer tooling — products used by sophisticated users who are often willing to work around rough edges. This masks quality problems. Friction logging surfaces what users tolerate and normalize, not just what they complain about.

Singleton argues that the level of craft visible in great products comes from this kind of systematic self-scrutiny. The products that feel "magical" are usually not architecturally different from their competitors — they've just had more friction methodically removed. At Stripe, engineering culture prizes meticulous craft, and friction logging is one mechanism for operationalizing that value.

### The Broader Principle

Friction logging is an instance of a wider principle: **product-minded engineering**. Engineers who regularly experience their own product as users develop better product intuitions, file better bugs, and make better implementation trade-offs. Friction logging creates structured occasions for this without requiring engineers to have a "product mindset" by nature — the process develops it.

### Variants

- **Customer friction logs**: Have customer success and support teams log friction on behalf of users
- **New employee logs**: Ask new hires to document friction during onboarding — they see things veterans have become blind to
- **Competitive friction logs**: Do the same exercise with competing products

## Sources
- [[david-singleton]] — "Meticulous craft in product development; friction logging as a quality practice" (Lenny's Podcast, 2025-01-16)

## See Also
- [[product-development-lifecycle]]
- [[minimum-lovable-product]]
- [[taste-as-competitive-advantage]]
- [[david-singleton]]
