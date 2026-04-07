---
aliases: []
guests: [asha-sharma, aparna-chennapragada]
---

# Product as Organism

> The shift from shipping static artifacts to building continuously learning, self-improving products powered by model feedback loops.

## Content

Articulated by [[asha-sharma]] at Microsoft, this concept describes a fundamental architectural and strategic shift in how products are built and what they are.

### The Old Model: Product as Artifact
- Ship a feature → improve incrementally → monitor a dashboard
- Product capability is fixed between releases
- IP lives in the code
- Improvement is driven by engineer decisions

### The New Model: Product as Organism
- Product interacts with users → data is captured → model is fine-tuned → product improves
- Product capability improves continuously without new releases
- IP lives in the trained model and the feedback loop infrastructure
- Improvement is partially autonomous

### What Makes It Possible
1. **Foundation models** capable enough to be fine-tuned on domain-specific data
2. **Post-training** (RLHF, RLAIF, DPO) that makes optimization on specific outcomes tractable
3. **Tool-calling / function-calling** models that can take action, not just generate text
4. **Falling cost** of inference and fine-tuning

Asha cites a study by Nathan Lambert: once a model hits 30B parameters, pre-training ROI declines rapidly; post-training on your own data becomes the better investment.

### The New "KPI": Product Metabolism
For teams building organisms, the key question is no longer "what's our DAU?" but "how fast can we complete the feedback loop?" — ingest interaction data → apply rewards model → fine-tune → evaluate → deploy.

### Real Example
Microsoft's Dragon medical product: moved from ~30–60% character acceptance rate (how often physicians accepted AI-suggested text) to 83% by annotating 600,000 patient-physician interactions with domain experts and feeding that back into the model continuously. This was not done by a large traditional product team, but by a small cross-functional squad focused entirely on the loop.

### Implications for Teams
- **New IP is the feedback loop**, not just the codebase
- **Full-stack builders** who can own the loop across ML, product, and data are more valuable
- **Observability** becomes a culture, not an ops task — you can't improve what you can't measure
- **Functions blur** — the distinction between PM, data scientist, and ML engineer shrinks when you're all optimizing the same loop

## Sources

- [[asha-sharma]] — "These are living organisms that just get better with the more interactions that happen. I think this is the new IP of every single company." (How 80,000 companies build with AI)
- [[aparna-chennapragada]] — "The time to first demo is much shorter, but the time to full deployment will take longer. The bar for scale is much higher." (Microsoft CPO)

## See Also

- [[asha-sharma]]
- [[ai-products]]
- [[ai-non-determinism]]
- [[experimentation-culture]]
