---
name: Pre-Mortem Framework
guests: [shreyas-doshi]
aliases: [pre-mortem, tigers-paper-tigers-elephants]
---

# Pre-Mortem Framework

> A structured meeting run before a product launch or initiative where the team imagines it has already failed, then works backwards to identify what went wrong — surfacing threats that psychological safety alone never would.

## Overview

The pre-mortem idea comes from research by Gary Klein (published in Harvard Business Review). Shreyas Doshi popularized a specific implementation used at Stripe and in his advisory work, combining Klein's core inversion prompt with a named taxonomy that becomes shared team vocabulary.

The insight: post-mortems are valuable, but why wait for failure to extract the same insights? A pre-mortem lets you do the work cheaply, before the damage occurs. Unlike a standard risk review ("what could go wrong?"), the hypothetical-failure framing unlocks psychological safety — nobody wants to be the pessimist, but everyone can speak freely when the premise is "imagine we already failed."

## Components

### The Prompt

The meeting leader opens with: *"Imagine this project/launch has miserably failed six months from now. Let's work backwards from that outcome. What went wrong?"*

The inversion is essential. It's not "what could go wrong?" (which keeps people in optimistic mode). It's "what did go wrong?" — a done deal, no longer hypothetical.

### The Taxonomy

Each participant contributes three types of items (entered silently and privately first):

- **Tiger**: A real threat that could kill the project — like a tiger would.
- **Paper Tiger**: A seeming threat that others worry about but you are not worried about. Useful for clearing the air on over-indexed concerns.
- **Elephant in the Room**: The uncomfortable assumption nobody is discussing. May not kill the project, but everyone can sense the problem nobody is naming.

### The Process

1. **Set the prompt** — leader opens with the hypothetical failure framing
2. **Quiet individual input** — 5–10 minutes of silent writing in a shared document (no one sees others' entries until they submit). This prevents anchoring and groupthink.
3. **Round-robin sharing** — go around the room, read entries
4. **Voting** — each person identifies the *other person's* tiger that they find most concerning (not their own). Surfaces consensus concerns.
5. **Prioritization** — the pre-mortem leader synthesizes a pre-mortem action plan and owns follow-through

### Scope

For large launches: run **two separate pre-mortems** — one for product/engineering risks, one for go-to-market risks (sales, marketing, support). For smaller launches: combine.

## How to Apply

- **When to run**: Early in a project or initiative, not at the finish line. Run it when you still have time to act on what you find.
- **Who to invite**: Every function involved in the launch. For engineering pre-mortems: all engineers plus PM and design. For GTM pre-mortems: sales, support, marketing, design, key engineering leads.
- **Artifact**: Use a shared doc (Shreyas built a Coda template). The output is a list of prioritized risks and an action plan with owners.
- **After the meeting**: The pre-mortem leader creates the action plan and holds themselves accountable for it. The group should not expect the problems to self-resolve.

## Why It Works

The post-mortem on failed launches often produces the insight "but someone knew about this." Pre-mortems give that person a container to speak. The two mechanisms are:

1. **Psychological safety via framing**: Negativity is invited and licensed by the prompt. You're not a doomsayer; you're playing the role the meeting asks you to play.
2. **Shared vocabulary**: After a few pre-mortems, "I have a tiger" becomes acceptable language in any meeting. The safety generalizes beyond the formal ritual.

## Sources
- [[shreyas-doshi]] — "The art of product management | Shreyas Doshi (Stripe, Twitter, Google, Yahoo)"

## See Also
- [[shreyas-doshi]]
- [[three-levels-product-work]]
- [[lno-framework]]
- [[decision-log]]
