---
concept: AI-First Product Development
guests: [tomer-cohen]
topics: [ai, product-management, organizational-transformation, linkedin]
---

# AI-First Product Development

## Definition
A mindset and organizational operating model where AI is treated as a core strategic driver — shaping product objectives, team structure, hiring, data strategy, and infrastructure decisions — rather than a feature layer applied on top of an existing product. "AI-first" is not about adding AI features; it's about re-deriving what you're building from the ground up given AI capabilities, and ensuring product leaders (not just engineers) own the algorithm's objective function.

## Guest Perspectives

### Tomer Cohen (via [[tomer-cohen]])
Cohen pioneered AI-first thinking at LinkedIn starting around 2016 — well before it became industry terminology. His framing:

**The two failure modes of AI in product organizations:**
1. Treating AI as a black box delegated to the engineering/ML team, where product leaders don't understand the objective function, features, or training data
2. Starting from technology ("we have this cool capability, what can we do with it?") rather than strategy ("what problem are we solving, and how does AI enable that better?")

**The river raft metaphor**: In an AI-powered marketplace or feed product, AI holds the two steering paddles that navigate the boat. If the product leader isn't holding those paddles, something else is steering the product. Most organizations have the guide (product leader) focused on the UI and not the engine.

**What product leaders must own:**
- The algorithm's objective function (what is it actually optimizing for? Can you write it on a whiteboard?)
- The features fed into the algorithm (not UI features — training features/signals)
- The data collection and fine-tuning strategy
- Infrastructure choices that affect product outcomes (often the highest-leverage lever, more impactful than building another UI button)

**LinkedIn's AI-first transformation (Fall 2022):**
1. All product leaders called to a session; asked to set aside existing roadmaps
2. Return in two weeks having re-thought problem statements with LLM capabilities assumed
3. Diverge phase: teams explore freely for weeks — some duplication is fine, learning is the goal
4. Converge phase: leadership picks top 4–5 bets, resources concentrated, weekly review cadence
5. Prompt engineering became an internal playbook; findings shared with OpenAI and Microsoft

**Controlling ingredients, not experience**: In deterministic products, the PM specifies every screen, flow, and default. In AI-powered products, the PM specifies the ingredients (objectives, constraints, data, guardrails) and the AI renders the experience. This requires a fundamental change in how PMs think about their job.

**From matchmaker to front stage**: LinkedIn's original AI was purely a back-end matchmaker (connecting job seekers with jobs, matching buyers with sellers) that users never saw. The post-GPT shift brought AI from the back of marketplaces to the front — where users directly interact with it as a co-pilot, coach, and interface layer.

**LinkedIn Coach example**: A job seeker cried during a product review, saying "I cannot share my journey with anybody." LinkedIn's Coach feature (accessible via the job tab) gives job seekers a personalized LLM-powered advisor — discussing fit, how to apply, comparing opportunities, emotional support — that removes the loneliness of job searching for people who can't afford a human coach.

## Key Insights
- AI-first is a mindset shift before it's a technology investment. The question is always "how does AI change the optimal answer to our product strategy?"
- Product leaders who don't own the algorithm can't lead AI-powered products effectively. ML engineering that isn't unified with product objectives will optimize for different goals.
- The diverge-then-converge approach prevents both premature lock-in (bad convergence) and unfocused exploration without accountability (bad divergence).
- Fine-tuning strategy is a product decision, not an engineering decision. Ignore it and your AI will optimize for what it was trained on, not what your product needs.

## Sources
- [[tomer-cohen]] — LinkedIn's AI-first transformation, starting 2016; post-GPT organizational reset in Fall 2022

## Related Pages
- [[tomer-cohen]]
- [[experimentation-culture]]
- [[product-ops]]
