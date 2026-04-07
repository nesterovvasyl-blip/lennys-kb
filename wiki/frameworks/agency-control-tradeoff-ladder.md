---
author: aishwarya-naresh-reganti-kiriti-badam
guests: [aishwarya-naresh-reganti-kiriti-badam]
---
# Agency-Control Tradeoff Ladder

> Staged AI deployment: each version increases agent autonomy while decreasing human oversight — move up only when the current stage is calibrated.

## Content

The Agency-Control Tradeoff Ladder is a deployment philosophy for AI agents that treats autonomy as something earned through demonstrated reliability, not assumed at launch.

### The ladder structure

Each rung represents a version of the system with higher agency and lower human control:

| Stage | Example (customer support) | Human role |
|-------|---------------------------|------------|
| V1 — Route/Classify | Assign tickets to the right queue | Humans handle everything; AI just sorts |
| V2 — Copilot/Draft | Generate draft responses for human review | Humans approve before sending |
| V3 — Autonomous | Resolve tickets end-to-end without review | Humans review escalations and monitor |

### The governing rule

**Do not advance to the next rung until the current rung is calibrated.** Calibration means:
- Error rates are understood and within acceptable bounds
- Failure modes have been characterized
- Monitoring is in place to detect drift

Skipping rungs — deploying a V3 system before V1 and V2 are proven — is the most common source of AI product failures.

### Connection to CC/CD

The Calibration Loop from [[continuous-calibration-continuous-development]] is what makes it safe to climb the ladder. Each loop through production data builds the confidence needed to graduate to the next rung.

## Sources

- [[aishwarya-naresh-reganti-kiriti-badam]] — "Move up only when current stage is calibrated." (episode title unknown)

## See Also

- [[continuous-calibration-continuous-development]]
- [[human-algorithm-interface]]
