---
aliases: []
episode_title: "OpenAI's CPO on the biggest AI product opportunities, model maximalism, and what makes a great AI PM"
publish_date: 2025-04-10
youtube_url: https://www.youtube.com/watch?v=scsW6_2SPC4
topics: [ai-products, product-management, product-leadership, openai, ai-strategy]
---

# Kevin Weil

> Chief Product Officer at OpenAI. Former CPO at Instagram and Twitter. Previously led Facebook's crypto project (Libra/Novi).

## Bio

Kevin Weil is CPO at OpenAI, having previously served as CPO at Instagram and held senior product roles at Twitter. He led Facebook's Libra cryptocurrency project before joining OpenAI. He's in a unique position to speak about AI product strategy: he was building AI products at Instagram when AI was a supporting capability, and now works at the frontier where AI is the entire product.

## Key Ideas

### Evals as the Core PM Skill in AI

In traditional software, "does it work?" is usually answerable through testing. In AI, you're deploying probabilistic systems where behavior varies by input. The fundamental skill shift for AI PMs: knowing how to build, use, and interpret **evaluations** (evals).

Evals are systematic tests that measure how well an AI system performs across a wide range of inputs. Good evals:
- Are comprehensive (cover edge cases and failure modes)
- Are measurable (give you a signal you can track over time)
- Are aligned with what users actually care about, not just what's easy to measure

Kevin's view: a PM who can't define, run, and reason about evals can't manage AI products effectively. This is as fundamental as knowing how to read metrics was for the previous generation of PMs.

### Model Maximalism

Kevin's strategic framework for building AI products: **build for where model capabilities are going, not where they are today**.

Most product teams are constrained by current model performance. Kevin argues this is the wrong constraint — models improve faster than products. If you build a product that's designed for today's model capabilities, it'll be outdated by the time you ship. Instead, imagine what the product would be if models were dramatically more capable, and build that.

He calls this "model maximalism" — assuming maximum reasonable model progress and designing products accordingly.

The risk: you can build something that doesn't work today and has to wait for model improvements. The reward: when model capabilities catch up, your product is ready.

### Iterative Deployment Philosophy

A principle OpenAI applies: deploy incrementally to get real-world feedback, then improve. Don't wait for the product to be perfect before shipping. The real world generates edge cases and failure modes that internal testing never will.

This is conventional for software, but more controversial for AI systems where failures can be more visible and potentially more harmful. Kevin's view: iterative deployment is even more important for AI precisely because the failure modes are harder to predict. You need real users to find them.

### Chat as Universal LLM Interface (for now)

Kevin observes that chat has become the default interface for LLMs — not because it's optimal, but because it's the most flexible. Chat can handle almost any task type. But he's explicit that this is a transitional UI: as AI gets embedded into more specific workflows, specialized interfaces will outperform general chat.

The opportunity for product builders: design for the specific workflow, not for generic chat. What does a purpose-built UI for your specific use case look like when chat is no longer the constraint?

### Deep Research as Breakthrough Product

Kevin highlights OpenAI's "Deep Research" product as one of the most significant releases — a product that can spend hours autonomously researching a topic, following leads, reading sources, and synthesizing. His excitement is about the underlying pattern: agentic workflows that complete long-horizon tasks.

This is different in kind from single-turn AI (ask a question, get an answer). Deep Research showed that users will trust AI with multi-step, extended tasks if the output quality is high.

### Vibe Coding and the Democratization of Software

Kevin is enthusiastic about vibe coding — the practice of writing software through natural language prompts to AI, without writing code directly. His view: this expands who can build software, not just who can build it faster.

The implication for PMs: the boundary between "I want this feature" and "I built this feature" will collapse for many PMs who learn to use vibe coding tools. PMs who can prototype their own ideas are fundamentally more effective.

### The Libra Failure

Kevin led Facebook's Libra cryptocurrency project, which was ultimately killed by regulatory pressure. His reflection: the idea was sound but they fundamentally misread the political and regulatory landscape. Building a global financial system requires a different kind of stakeholder management than building consumer products — one where governments are veto players, not just critics.

Lesson: for products with existential regulatory risk, the regulatory strategy needs to be a first-class product discipline, not an afterthought.

## Memorable Quotes

- "The PM skill for the AI era is knowing how to build and use evals. It's as fundamental as reading metrics was for the last generation."
- "Build for where model capabilities are going, not where they are today. That's model maximalism."
- "Chat is the transitional interface. It's flexible, but it's not optimal for specific workflows."
- "Deep Research showed that users will trust AI with multi-hour, multi-step tasks if the quality is there."
- "Vibe coding isn't about faster software — it's about more people being able to build software."
- "On Libra: we misread the regulatory landscape. Governments are veto players, not critics."

## Actionable Advice

- If you're a PM building AI products, invest seriously in eval design — it's your most important technical skill
- Apply model maximalism: design your product for significantly more capable models than exist today
- For products with regulatory exposure, make regulatory strategy a first-class product discipline from day one
- Experiment with vibe coding for prototyping your own product ideas

## Topic Tags

ai-products, ai-evals, model-maximalism, openai, product-leadership, vibe-coding, ai-product-management

## See Also

- [[ai-evals]] — existing concept page; Kevin adds a senior PM perspective
- [[model-maximalism]] — concept page
- [[kayvon-beykpour]] — both worked at Twitter
- [[keith-coleman-jay-baxter]] — also worked at Twitter/X
- [[chip-huyen]] — complementary ML/AI engineering perspective
