---
aliases: []
guests: [aishwarya-naresh-reganti-kiriti-badam]
---

# AI Non-Determinism

> Unlike traditional software, AI products face unpredictability on both sides: unbounded natural language inputs and probabilistic model outputs.

## Content

Traditional software products operate on a deterministic contract: given input X, the system reliably produces output Y. Engineering and product disciplines were built around this assumption — specifications, test suites, and acceptance criteria all depend on predictable behavior.

AI products break this contract in two directions simultaneously:

1. **Input unboundedness**: Users interact via natural language, which is effectively infinite in variety. There is no finite set of valid inputs to test against or design for.
2. **Output probabilism**: Model outputs are probabilistic — the same prompt can yield different results across runs, and edge-case outputs are structurally unavoidable.

This creates a new design and engineering challenge: you cannot fully specify correct behavior in advance. Instead, product teams must shift toward **behavior calibration** — iteratively shaping how the system tends to behave across the distribution of likely inputs, using techniques like:

- RLHF and preference tuning
- Guardrails and output filters
- Evaluation frameworks (evals) that sample from real usage
- Human-in-the-loop review for high-stakes outputs

The implication for product managers: success metrics, QA processes, and launch criteria all need to be rethought for probabilistic systems.

## Sources

- [[aishwarya-naresh-reganti-kiriti-badam]] — "Requires designing for behavior calibration rather than specification" (AI product design episode)

## See Also

- [[taste-as-competitive-advantage]]
- [[experimentation-culture]]
