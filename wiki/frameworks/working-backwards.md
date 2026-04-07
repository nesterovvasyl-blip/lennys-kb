---
author: Amazon (popularized); documented by Bill Carr; adapted by Anuj Rathi and Ian McAllister
guests: [anuj-rathi, bill-carr, ian-mcallister]
---

# Working Backwards

> Start with the press release for the finished product, then work backwards to figure out how to build it.

## Content

Working Backwards is Amazon's product development framework: before writing any specs or starting any engineering, the team writes a mock press release announcing the finished product as if it were already shipped. This forces clarity on what success actually looks like from the customer's perspective, and surfaces misalignment early when the cost to fix it is low.

The standard process:
1. Write a press release describing the finished product's customer benefit in plain language
2. Write a FAQ anticipating customer and internal objections
3. Use the PR/FAQ as the alignment document — what you're building toward, not a spec of how

**[[anuj-rathi]]'s adaptation** at Swiggy and Jupiter Money added a key twist: always write **three divergent press releases** before committing to one direction. This forces genuine exploration of different strategies (not just variations on the same idea), gives leadership a structured way to compare trade-offs, and ensures PM recommendations are informed and defensible. The FAQs within each PR FAQ can also double as pre-launch checklists for compliance, marketplace impact, and edge cases.

**[[bill-carr]]'s account** from building this process at Amazon adds important context: the PR/FAQ was developed in the 2003–2007 window when Amazon transitioned from startup to scaled enterprise. The PR/FAQ replaced lengthy planning documents and roadmap debates that were based on deeply flawed assumptions. Carr emphasizes that the artifact is deliberately written in *customer language*, not technical language — if you can't explain what you're building in a press release a customer would understand, you don't yet know what you're building. The companion FAQ forces you to anticipate both customer and internal objections before any engineering begins.

**[[ian-mcallister]]'s key distinction** from his time at Amazon: working backwards is a **mindset**, not just a **mechanism**. The mechanism is the PR/FAQ artifact. The mindset is: start from the customer's desired outcome and work backwards to what to build — rather than starting from available technology and looking for a use case. He calls the reverse approach "technology in the pantry" thinking — you have a capability, you look for a problem it could solve. This is backwards. The PR/FAQ enforces the mindset for people who don't have it yet. For PMs who already think customer-first, the artifact is optional; the mindset is not.

## Sources
- [[anuj-rathi]] — "Work backwards from an amazing future. Be paranoid about everything that could go wrong." (The full-stack PM)
- [[bill-carr]] — "Start with what's best for the customer and come backward from there — that informs what work you have to do to create the solution." (Unpacking Amazon's unique ways of working)
- [[ian-mcallister]] — "What separates good product managers from great ones" (working backwards as mindset vs. mechanism)

## See Also
- [[anuj-rathi]]
- [[strategy]]
- [[growth]]
