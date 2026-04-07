---
aliases: [outcome-based-pricing, resolution-based-pricing, beautifully-simple-pricing]
guests: [bret-taylor, brian-balfour, eoghan-mccabe]
---

# Outcomes-Based Pricing

> A pricing model in which the customer pays when the product successfully accomplishes a defined business outcome — aligning vendor and customer incentives and making ROI self-evident.

## Content

Outcomes-based pricing charges for results, not access. Unlike seat-based (SaaS) or usage-based (tokens, API calls) pricing, it answers the question "did this actually accomplish what you needed?" with a measurable, attributable transaction.

### Why AI Agents Enable Outcomes-Based Pricing (Bret Taylor)

Bret Taylor argues this is the inevitable direction for all AI software, and Sierra (his AI agent company) demonstrates it concretely. Sierra builds customer-facing AI agents for companies like ADT and Sonos. When the agent successfully resolves a customer service interaction without a human picking up the phone, that's a "resolution" — and Sierra charges per resolution, with a pre-negotiated rate.

Why this only works for agents:
1. **Autonomy**: The agent actually does the job, not just assists. A human didn't have to intervene. This makes attribution clean — either it was resolved or it wasn't.
2. **Measurability**: The outcome is unambiguous. Customer issue resolved = yes or no. No attribution model needed.
3. **Comparison point**: The enterprise already knows what the alternative costs ($10–$20 per phone call with a human agent). The savings are immediately visible.

### The Problem with Usage-Based Pricing for AI

Taylor uses a pointed analogy: "There's a famous story of an Apple engineer whose bad manager asked him to report how many lines of code he wrote every day. He submitted a negative number when he did a big refactoring." Tokens are like lines of code — a bad proxy for value. You can use a lot of tokens and produce negative value (long phone call that ends without resolution, customer rates it negatively, calls again). The activity and the outcome are not correlated.

### The Business Case for Vendors

Outcomes-based pricing transforms vendor-customer relationships from "we sold you software" to "we are your partner in achieving X." Taylor: "Every technology company aspires to be a partner, not a vendor. At Sierra, we are truly a partner to every single one of our customers because we're all aligned on what we want to achieve."

The vendor's incentives shift fundamentally: you can't just throw software at the wall because you'll never get paid if it doesn't work. This creates a company structure deeply oriented around helping customers achieve outcomes.

### Durability Question (Brian Balfour)

Balfour raises a counterpoint: outcomes-based pricing may have a durability problem as competition increases. If many vendors offer resolution-based pricing for customer service agents, competition will erode the per-resolution rate over time — from $15 toward $5 toward $1. The pricing power is only durable if paired with a real moat (data advantage, integrations, quality gap). Without a moat, competition will commoditize the outcome itself.

Taylor's implicit response: Sierra's moat is the accumulated data and customer-specific context from handling millions of interactions, plus the quality of its agent platform. This is the data network effect that could sustain pricing power.

### When Outcomes-Based Pricing Is Possible

- The agent must be autonomous (acting, not just suggesting)
- The outcome must be measurable (binary or clearly quantifiable)
- There must be a clear comparison point for the customer (what did this replace?)

Not all AI applications meet these criteria. Coding assistants that help engineers think faster are hard to price on outcomes — you can't attribute a feature shipping to any single AI intervention. This is why coding tools tend to be seat-based or usage-based.

### Eoghan McCabe: $0.99 Per Resolved Ticket at Intercom

McCabe is the most concrete implementation example in the canon. Intercom priced its AI agent Fin at $0.99 per successfully resolved customer ticket — a complete departure from Intercom's existing seat-based SaaS model. McCabe's framing: "beautifully simple pricing." The customer already knows the comparison point — a human agent costs $10-20 per ticket. At $0.99, the ROI math is instant and self-evident. If Fin doesn't resolve the ticket (the customer has to escalate to a human), Intercom doesn't charge. This creates pure incentive alignment: Intercom only makes money when the product works.

The implementation required courage because it meant cannibalizing their existing seat revenue. Intercom was betting that the volume of AI-resolved tickets at $0.99 would exceed the revenue from seats they'd replace. McCabe describes this as a "first-principles" decision — ignoring what the business currently earned and asking what was true about what customers actually wanted to pay for.

## Sources
- [[bret-taylor]] — "The whole market is going to go towards outcomes-based pricing. It's just so obviously the correct way to build and sell software." (He saved OpenAI, invented the 'Like' button, and built Google Maps)
- [[brian-balfour]] — "Competition erodes that away... unless there's something else that creates durable pricing power." (Why ChatGPT will be the next big growth channel)
- [[eoghan-mccabe]] — "Fin at 99 cents per resolved ticket. That is the most honest pricing I've ever seen in software. You pay when it works." (The art of the AI pivot: Intercom's journey to becoming an AI-first company)

## See Also
- [[bret-taylor]]
- [[brian-balfour]]
- [[ai-products]]
- [[strategy]]
