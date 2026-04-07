---
aliases: [friction log, friction audit]
guests: [katie-dill, karri-saarinen]
---

# Friction Logging

> The practice of systematically documenting every point of confusion, friction, or failure while using a product as a user — used to surface quality issues that automated testing and team demos miss.

## Content

Friction logging is a hands-on quality practice: a leader or team member uses their own product as a real user would, writing down everything that feels slow, confusing, broken, or jarring. The output is a prioritized list of real-world quality gaps — often including issues that live at the seams between teams, which no single team would otherwise surface.

### Katie Dill's Version: Walk the Store

At Stripe, Katie Dill (Head of Design) embedded friction logging into the [[walk-the-store]] process. Journey owners — senior leaders responsible for specific end-to-end user flows — periodically experience their journey as a user, logging friction as they go. The key properties:
- **First-person and visceral**: doing, not watching (no demos or screen recordings)
- **End-to-end**: following the actual user journey, not just testing a single feature
- **Cross-functional surface**: issues at team boundaries (e.g., SEO copy contradicting product copy) get surfaced that neither individual team would catch
- **Score and calibrate**: owners score journey quality and calibrate scores together, building a shared quality language across the organization

### Karri Saarinen's Version: Ship Ugly to Yourself

At Linear, Karri Saarinen (co-founder and CEO) uses a complementary practice: new features are shipped to internal staging within the first week of development — before designs are finalized. Then 1-5 willing customers co-create in an early access state. Only at general release does the full quality bar apply. This structure means the team is always "friction logging" on real, working software, not polished demos.

Karri's core point: you cannot identify quality issues through design review or code review alone. The only way to find janky animations, broken flows, and UX debt is to *use* the product. "In design reviews, go experience the product yourself rather than just reviewing in demos — only visceral use reveals bugs, janky animations, and broken flows."

### Why It Works

Most quality-review processes are asynchronous and filtered: user reports, bug tickets, analytics. These catch obvious problems but miss the subtle degradation that accumulates over time — the onboarding that was good a year ago but now has three extra steps from three different teams adding features. Friction logging is synchronous and unfiltered: you feel the product the way users do.

The practice pairs well with metrics: metrics tell you *that* something is underperforming; friction logging tells you *why*.

## Sources

- [[katie-dill]] — "Building beautiful products with Stripe's Head of Design | Katie Dill (Stripe, Airbnb, Lyft)" (2023-10-15)
- [[karri-saarinen]] — "Inside Linear: Building with taste, craft, and focus" (2023-10-08)

## See Also

- [[walk-the-store]]
- [[product-craft]]
- [[taste-as-competitive-advantage]]
- [[design-tenets]]
