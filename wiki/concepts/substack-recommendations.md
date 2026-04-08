---
concept: Substack Recommendations
guests: [sachin-monga]
topics: [growth, network-effects, creator-economy, viral-loops, subscriptions]
---

# Substack Recommendations

> Substack's writer-controlled cross-promotion feature — arguably one of the most effective viral growth mechanisms in creator economy history — and the product philosophy behind why it was built the way it was.

## Overview

Substack Recommendations allows writers to publicly recommend other newsletters. When a reader subscribes to any Substack, they see a curated list of recommendations from that writer. The mechanism is fully writer-controlled: each writer picks their own list, and there is no algorithmic ranking or Substack-curated suggestions.

At time of recording (October 2022), the feature had driven millions of new subscriptions across tens of thousands of unique writers, with 1 in 3 new subscriptions on the platform coming from the Substack network.

## The Product Decision That Made It Work

The most important feature of the recommendations product is what it is *not*: it is not an algorithmic recommendation engine. Substack deliberately chose not to build the obvious version of this — a "people you may also like" unit that Substack's own algorithm would populate — because that would violate the platform's core principle of writer control.

Sachin Monga describes the design decision: "The most obvious way would be something like 'here are some Substacks you might like' — we could have done People You May Know. That kind of thing drove very non-trivial Facebook growth in the early days. We could have done that. But then the writer who owns that space is not really in control."

The writer-controlled approach looked harder (more steps to adoption, more dependencies on writer quality). Chris Best (CEO) was initially skeptical it would get enough adoption to matter. It took off faster than anyone expected.

## Why It Works

Three interlocking dynamics:

1. **Trust transfer.** The recommendation comes from a specific writer a reader already trusts, not from an algorithm. This creates higher-quality signal and higher-intent subscribers.

2. **Goodwill viral loop.** When Writer A recommends Writer B, Writer B gets an email saying "Lenny is recommending you, and here's how many readers he's sending you." This creates a social incentive to recommend generously — you're doing something visibly good for another creator.

3. **Surface area is the subscribe moment.** Recommendations appear precisely when a reader is already making a subscription decision. This captures maximum conversion intent.

## The "Build With Writers" Principle

The recommendations feature was developed using what Sachin calls the "build with writers" philosophy — a product development principle at Substack. Rather than just build and ship, the team:
1. Mocked up the feature concept
2. Called 10 writers for qualitative feedback
3. Ran a small pilot before general rollout
4. Built a "Product Lab" of ~100 writers for ongoing early access

The feature that shipped on day one was meaningfully different from what the team had initially imagined — the pilot surfaced changes that made it work. This process has become a default at Substack for any feature that fundamentally changes how the platform operates.

## Future Direction

Sachin hints at the next phase: treating recommendations not just as a subscribe-flow step but as a social graph. The existing recommendations data represents a web of trust and influence among writers that could be used for much more — surfacing recommendations to existing subscribers who already trust a writer, not just to brand-new ones discovering that writer for the first time.

## Actionable Takeaways
- When building discovery features, ask which version preserves user/creator control rather than defaulting to the algorithmic approach
- Counter-intuitive but true: the harder-to-adopt, more opt-in version often outperforms because it generates higher-trust signals
- The goodwill loop is an underappreciated viral mechanic: reward the person doing the recommending, not just the recommended person
- Run pilots with real users before general rollout — the output will change in ways that matter

## Sources
- [[sachin-monga]] — "Building Substack" (2022-10-30)

## See Also
- [[network-effects]]
- [[viral-growth-loop]]
- [[creator-economy]]
- [[word-of-mouth-growth]]
