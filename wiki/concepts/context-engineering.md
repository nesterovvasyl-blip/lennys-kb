---
aliases: [context window engineering, context design]
guests: [dan-shipper]
---

# Context Engineering

> The practice of carefully constructing the context window you give an AI model — selecting documents, examples, instructions, and constraints — to maximize output quality for a specific task.

## Content

Context engineering is an emerging term of art for the skill of working with AI models at the system level, not just the prompt level. Dan Shipper ([[dan-shipper]]) popularized the term at Every, his AI-native media and software company.

### Context Engineering vs. Prompt Engineering

Prompt engineering operates at the level of a single instruction: "Write a PRD for feature X in the style of Y." Context engineering operates at the level of the full context window: what background documents, examples, prior conversation, constraints, and role definitions does the model need to do this work well, consistently, across many sessions?

The distinction matters because:
1. **Models are highly sensitive to context**: The same model given the same prompt but different context can produce dramatically different quality outputs. The context isn't just "background" — it's part of the instruction.
2. **Context is composable**: A well-designed context package (documents + examples + constraints) can be reused across many prompts, creating leverage. This is closer to software design than instruction writing.
3. **Context selection is a skill**: Knowing what to include, what to exclude, and how to format the included material for the model's "understanding" is a non-obvious discipline.

### Components of a Good Context Package

- **Domain documents**: Relevant background material the model needs to know but won't have from training alone (company-specific terms, product specs, customer data)
- **Examples (few-shot)**: 2-5 examples of the desired output quality and format — the single most effective technique for shaping model behavior
- **Constraints**: Explicit instructions about what the model should not do (format restrictions, tone guidelines, things to avoid)
- **Role definition**: A clear statement of what the model is acting as, which primes it to draw on relevant knowledge patterns
- **Success criteria**: What does a good output look like? Including this explicitly helps the model self-evaluate before responding

### Why This Skill Grows in Importance

Shipper's observation: as models get more capable, the limiting factor shifts from model capability to context design. A more capable model given poor context produces mediocre output. A less capable model given excellent context often outperforms the more capable model. As the baseline capability ceiling rises, context engineering becomes the primary lever for differentiation.

At Every, Shipper uses context engineering as the foundation of their AI product development: before building any AI feature, the team designs the context package. This is analogous to how a software team designs an API before implementing it.

## Sources
- [[dan-shipper]] — "Context engineering is the skill. How you construct the context window — what you include, what you exclude, how you frame the task — determines 80% of the output quality." ("How AI is changing the way we build products")

## See Also
- [[ai-products]]
- [[ai-operations-role]]
- [[ai-evals]]
