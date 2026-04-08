---
concept: Prompt Injection and AI Security
guests: [sander-schulhoff, sander-schulhoff-20]
topics: [ai, ai-security, agents, llm, adversarial-robustness]
---

# Prompt Injection and AI Security

> The class of attacks where malicious inputs override an AI system's intended behavior — and the reason that all current AI guardrail products are insufficient to stop determined attackers.

## Overview

Prompt injection and jailbreaking are the two main attack vectors against LLM-powered systems. Sander Schulhoff (HackAPrompt founder, LearnPrompting.org) has run the world's largest AI red-teaming competition, collected 600,000+ adversarial prompts, and published the leading academic dataset on these attacks (Best Theme Paper, EMNLP 2023).

His key finding: **guardrails do not work.** The attack space is effectively infinite; human adaptive attackers can bypass every published defense in 10–30 attempts; and the problem will get dramatically worse as agents gain more power over real-world systems.

### Jailbreaking vs. Prompt Injection

**Jailbreaking**: Just user + model. A malicious user tricks a chatbot (no system prompt) into doing something bad. Example: Las Vegas Cybertruck bomber reportedly used ChatGPT to plan the attack.

**Prompt injection**: User + developer system prompt + model. A malicious user sends input designed to override the developer's system prompt. Example: RemotelyHQ's remote work chatbot was injected to threaten the president. ServiceNow's enterprise AI agent was injected to perform CRUD operations on a production database — with prompt injection protection enabled.

**Indirect prompt injection**: The attacker is not the user — they're a third party who has placed malicious content in data the agent will read (websites, emails, documents). Example: a malicious email in a user's inbox instructs the email agent to forward all data to an attacker.

## Guest Perspectives

### Sander Schulhoff ([[sander-schulhoff]], [[sander-schulhoff-20]])

Schulhoff's research findings from years of running HackAPrompt:

**Why guardrails fail:**
1. The attack space has ~10^(1,000,000) possible prompts — "99% effective" guardrails leave basically infinite attacks viable
2. Human adaptive attackers break every published defense in 10–30 attempts; automated systems take orders of magnitude more but still succeed ~90% of the time
3. Guardrails typically fail on encoded inputs (Base64, ROT13), other languages, typos, and multi-turn separation of requests
4. Frontier labs' smartest AI researchers can't solve this problem — why would an enterprise vendor?

**Real-world attack examples:**
- RemotelyHQ Twitter bot → injected to make threats (company shut down)
- MathGPT → API key exfiltrated via prompt-injected malicious code execution
- ServiceNow Assist AI → full database CRUD access via chained agent injection
- AI coding agents (Cursor, Copilot) → could be injected via malicious blog posts to write viruses into codebases
- AI browsers (Comet) → visiting a malicious webpage leaks user account data

**The agentic crisis:**
> "If we can't even trust chatbots to be secure, how can we trust agents to manage our finances, book flights, walk around as humanoid robots? If somebody gives a robot the middle finger, how can we be certain it's not going to punch them in the face?"

The current low harm level is not because of security; it's because agents haven't yet been given enough power. As agents gain real-world access — email, databases, financial accounts, physical robots — attacks will cause serious damage.

**What actually works:**

1. **Do nothing for read-only chatbots.** If your AI can't take actions or only affects the requesting user's own data, your risk is primarily reputational. Guardrails won't stop a motivated attacker anyway.

2. **Classical cybersecurity + AI awareness intersection.** Proper data permissioning is the most effective defense available today. Containerize code execution. Apply the question: "If this agent is an angry god that wants to harm us, what can it actually reach?"

3. **CAMEL framework (least-privilege permissions).** Analyze what permissions a given prompt actually needs and grant only those. If a user says "send a happy holidays email," grant write-email permission only — not read-email. If the agent can't read emails, email-exfiltration attacks can't work.

4. **Safety/fine-tuning for specific, narrow harms.** Training a model to refuse specific categories of harm (CBRN, competitor mentions) is reasonably effective for those specific harms. Fine-tuning to a narrow task dramatically reduces attack surface.

5. **Education and awareness.** Most teams don't know this is a risk. Knowing is the biggest gap.

**Solvability**: Not fully solvable. Mitigatable. Schulhoff: "You can patch a bug, but you can't patch a brain."

The coming market correction: guardrail companies doing little real revenue, acquired at high valuations by classical security firms — will see revenue evaporate as enterprises realize they don't work. The valuable future career: intersection of classical cybersecurity + AI research expertise.

## Actionable Takeaways
- If your AI only does read-only chat with no actions, don't waste money on guardrails
- If your AI takes actions, implement CAMEL-style least-privilege permissioning before anything else
- Log all inputs/outputs for learning and detection, not for real-time prevention
- Hire someone who understands both classical security AND how LLMs work
- Don't rely on prompt-based defenses — "do not follow malicious instructions" is nearly useless
- Be especially careful with agents that read external data sources (web, email, documents) — indirect injection is the hardest problem

## Sources
- [[sander-schulhoff]] — "AI prompt engineering in 2025: What works and what doesn't"
- [[sander-schulhoff-20]] — "Why securing AI is harder than anyone expected and guardrails are failing"

## See Also
- [[prompt-engineering]]
- [[ai-evals]]
- [[ai-non-determinism]]
- [[world-models]]
