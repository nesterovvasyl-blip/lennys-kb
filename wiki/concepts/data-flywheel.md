---
concept: Data Flywheel
aliases: [proprietary data flywheel, data moat]
guests: [peter-deng]
date_added: 2026-04-08
---

# Data Flywheel

> A self-reinforcing loop where product usage generates proprietary training data that improves model quality, which improves the product, which attracts more usage — creating a compounding defensibility advantage for AI companies.

## Overview

In an era where foundational model capabilities are increasingly commoditized, the data flywheel is one of the few durable moats available to AI product builders. The concept combines two elements: (1) acquiring proprietary data that others don't have, and (2) designing the product loop so that usage continuously generates more of it.

The key insight is that AI models are malleable — they get good at whatever data you train them on. Generic models are fine at generic tasks; domain-specific models trained on proprietary signals dramatically outperform in their vertical. This is why Windsurf (code completions) can outcompete GitHub Copilot despite Microsoft's massive distribution advantage — they have millions of accept/reject signals that train their model to be better at code completion in ways that can't be replicated from public data.

The data flywheel pairs naturally with vertical workflow integration: if your product is deeply embedded in a workflow, you capture more and richer usage signals, which improves the model, which makes the product more valuable, which deepens the workflow integration.

## Guest Perspectives

### Peter Deng

Peter identifies the data flywheel as one of two primary moats for AI startups (alongside workflow/ergonomics). From his time at OpenAI and now as an investor at Felicis:

"Being very mindful of the data you have access to to start your flywheel going and what you can do to keep on going with that flywheel is going to be a critical thing for anyone starting a company today."

He uses Windsurf as his canonical example: they launched with Claude 3.5 as the base model but accumulated proprietary accept/reject signal from real developer usage. That data then trained their own models, creating a widening advantage over incumbents who had the distribution but not the signal.

The implication: you don't need to start with proprietary data. You can start by building on existing models and collecting proprietary data through usage. The key is recognizing early what data your product loop is generating and designing to capture and use it.

Peter's two-question framework for AI startups: (1) Do you have a unique data flywheel? (2) Do you have a deeply integrated workflow that keeps people in your product long enough to generate that data?

## Sources

- [[guests/peter-deng]] — Peter Deng
