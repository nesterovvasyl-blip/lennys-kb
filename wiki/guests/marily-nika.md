---
guest: Marily Nika
role: AI Product Lead at Meta Reality Labs; lecturer on AI Product Management
episode: "AI and product management | Marily Nika (Meta, Google)"
date: 2023-02-05
topics: [ai-products, product-management, ai-for-pms, machine-learning]
---

# Marily Nika

> Computer scientist, PhD in Machine Learning, and former Meta/Google product leader who teaches the most popular AI product management course on Maven.

## Content

**Bio**: Marily Nika has a PhD in Machine Learning (2014) and spent over 8 years at Google working on Google Glass, computer vision, and speech recognition ML systems. She then moved to Meta's Reality Labs, working on AI for Metaverse, avatars, and identity. She teaches the most popular course on Maven on AI and product management, and has become a leading voice in how PMs should think about AI.

### Key Ideas

- **Every PM Will Be an AI PM**: Marily's central thesis is that AI is becoming the default layer of all products — personalization, recommendation, automation. PMs who don't understand AI will be at a disadvantage. The implication is not that PMs will write AI code, but that they'll increasingly work alongside research scientists who build models, and they need to know how to frame problems for AI development.

- **The Shiny Object Trap**: "Don't do AI for the sake of AI." The right sequence is: (1) identify a real user problem with a real pain point, (2) identify that AI is a genuinely good solution for it, (3) then figure out implementation. Never reverse this. For MVPs specifically — don't waste data scientist time training models. Fake the AI behavior in a Figma prototype. AI is for products that have already shown signal.

- **The AI PM vs. Generalist PM**: The generalist PM helps their team build and ship the right product. The AI PM helps their team solve the right problem — which requires deeper familiarity with probabilistic systems, uncertainty in research timelines, and fluency with data scientists.

- **Don't Build Your MVP with AI**: AI adds real complexity: training time, data requirements, probabilistic outputs, model iterations that take weeks. For early validation of a concept that might use AI, use Figma mockups to simulate AI behavior. Invest in real AI only when you have adjacent data to leverage and a validated audience.

- **How Models Work**: A model is like a child's brain being trained: show it thousands of labeled examples, let it find patterns (not human-legible decision trees — the brain just learns), and it develops the ability to classify or generate with a probability score attached. You train with lots of labeled data; the output is a set of weights that powers probabilistic inference.

- **When to Build Your Own Model vs. Use Existing APIs**: Large tech companies should build proprietary models for their core value — otherwise their quality is identical to every competitor using the same off-the-shelf dataset. For most startups, leverage existing models (GPT etc.) and focus on the application layer. The quality-vs-launch question ("Is 70% accuracy good enough for our users?") is squarely a PM decision, not a data scientist decision.

- **Skills PMs Should Develop**: Marily encourages PMs to learn to code and train small models — not to replace engineers, but to develop the "piano fundamentals" that give you a different mental model of how AI products work. Understanding the lifecycle of an ML project (scoping → data → training → evaluation → deployment) makes you a better collaborator with research teams.

- **AI Enhances, Doesn't Replace PMs**: AI frees up time from tedious tasks (writing PRD boilerplate, generating user segments, drafting mission statements) so PMs can focus on harder strategic and ethical questions — especially around viability: what is acceptable probabilistic error? When is AI-generated output mission-critical vs. best-effort?

### Actionable Advice

- Use ChatGPT to improve mission statements (not write them from scratch): draft yours, then ask it to rewrite for a broader audience, including people outside the product domain.
- Use ChatGPT to generate user segments: provide a product description, ask it for segments with motivations and pain points. It will surface user types you hadn't considered.
- Before investing in AI/ML, check: do you have data from an adjacent product or existing user behavior you can leverage? If no, wait.
- Start learning ML fundamentals through an online course — even basic hands-on training builds the confidence to understand what you're asking of your data science team.

### Notable Quotes

> "Don't do AI for the sake of doing AI. Make sure there is a problem there. Make sure there is a pain point that needs to be solved in a smart way."

> "The generalist PM helps their team and their company build and ship the right product. But the AI PM helps their team or company solve the right problem."

> "In the future, everything will be AI by default."

## Sources

- [[marily-nika]] — "AI and product management" (Lenny's Podcast, 2023-02-05)

## See Also

- [[ai-products]]
- [[product-management]]
- [[ai-for-pms]]
