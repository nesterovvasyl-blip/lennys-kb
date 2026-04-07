---
guests: [aishwarya-naresh-reganti-kiriti-badam, alexander-embiricos, alex-komoroske, amjad-masad, anton-osika, andrew-wilkinson, aparna-chennapragada, asha-sharma, bret-taylor, brendan-foody, brian-balfour, chip-huyen, dan-shipper, dhanji-r-prasanna, dr-fei-fei-li]
related_raw_index: ai.md
---

# AI Products

> Building AI products requires fundamentally different approaches from traditional software.

## Content

AI product development challenges assumptions carried over from deterministic software: outputs are probabilistic, workflows are emergent, and the bottleneck is often human trust rather than technical capability.

**Start low-agency, earn trust**
Aishwarya Naresh Reganti and Kiriti Badam advocate a "low-agency/high-control" starting posture for AI products. Rather than shipping maximally autonomous agents, teams should begin with AI that surfaces suggestions and waits for human confirmation — then gradually expand autonomy as trust is established. They describe this as a Continuous Calibration / Continuous Development (CC/CD) lifecycle, analogous to CI/CD in traditional software. A key insight: pain is the new moat. Products that deeply understand and solve a specific workflow pain point are more defensible than those built on model capability alone. 80% of successful AI builders spend the majority of their time understanding workflows — not building or fine-tuning models.

**The coding agent as the universal template**
Alexander Embiricos argues that any sufficiently capable agent should be built as a coding agent — or at least adopt the coding agent's design patterns. The reason: coding agents solve the fundamental challenges of agentic products (long-horizon tasks, error correction, verifiable outputs) better than any other agent type. He identifies human typing speed as the real bottleneck in human-AI collaboration, not model intelligence — which implies UI and interaction design matter more than most teams realize. "Meet users where they are" means embedding AI in existing workflows rather than asking users to adopt new tools.

**Taste as the new differentiator**
Alex Komoroske observes that LLMs function as "magical duct tape" — they can connect nearly anything to anything. When execution is commoditized, taste becomes the scarce resource. Teams that develop strong opinions about what makes a great experience, and can execute on those opinions repeatedly, will outperform teams that focus primarily on technical differentiation.

**AI as universal developer: Replit's thesis**
Amjad Masad argues the real opportunity isn't making engineers 20% better — it's making everyone a developer. Replit's agent builds full-stack apps from natural language prompts in minutes for pennies in compute cost. The key technical insight: AI agents need purpose-built interfaces (AI Computer Interfaces / ACI), not repurposed human interfaces. Replit gives its agent text-based shell views, specialized editor tools with error feedback, and structured service access. Current limitations: agents are excellent at building MVPs but struggle with large iterations and database migrations. Masad's prediction: in ~5 years, someone will run a billion-dollar company with zero employees.

**Jevons' Paradox and the software explosion**
Masad observes Jevons' Paradox in action: as AI drops the cost of building software, total software creation increases dramatically. People build things they never would have hired a developer for. The implication: the bottleneck shifts from production to ideation. "Being generative" — rapidly producing new ideas — becomes the scarce skill. SaaS may face pricing pressure as custom software becomes trivially cheap to create.

**AI as the universal builder**
Anton Osika's Lovable represents the next step: AI that doesn't just assist engineers but replaces the need for engineering entirely for many use cases. Lovable is an "AI software engineer" — describe an idea in English, get a working product in 30 seconds. Key technical insight: Lovable identified where AI gets stuck (login, data persistence, Stripe payments), painstakingly fixed those failure modes, and maintained fast quantitative feedback loops. The result: $10M ARR in 60 days with 15 people. Anton argues the bottleneck is shifting from engineering to taste and user understanding: "Being a generalist is much more important than it used to be." Engineers should see themselves as translators between human problems and technical constraints, abstracting up several levels from pure code.

**Prompting as a PM skill**
Both Osika and the Lovable demo reveal that clear communication — specifying exactly what you expect and what's not working — is even more critical with AI than with humans. This is fundamentally a product management skill: requirement definition, problem articulation, and feedback precision. The implication: PM skills become more valuable, not less, in an AI-driven world.

**AI as the $200/month employee**
Andrew Wilkinson provides a practitioner's perspective on AI agents in daily business operations. Using Lindy.ai, he has automated email triage (reducing volume 20%), calendar management, meeting prep (auto-researching attendees 30 minutes before meetings), CRM updates (auto-detecting contact cities from emails), and decision routing (AI presents simple decisions as multiple choice). He replaced a full-time assistant entirely with AI agents. His view on the current state: we're in the "Palm Treo phase" of AI -- powerful for technical users who can build agents, but not yet accessible to everyone. The "iPhone moment" -- when anyone can just talk to an AI employee -- is 1-5 years away.

**NLX is the new UX**
Aparna Chennapragada argues that natural language interfaces require as much explicit design as GUIs — just with invisible primitives: prompts, editable plans, progress visibility, follow-up suggestions. The common mistake is thinking "the model eats the product, so there's nothing to design." Teams need to develop NLX design skills. See [[nlx-natural-language-experience]].

**Product as organism**
Asha Sharma at Microsoft sees a shift from products as static artifacts to products as organisms — continuously learning through feedback loops, fine-tuning, and rewards models. The new IP of every company is the speed of its feedback loop. Post-training (fine-tuning on proprietary interaction data) is where differentiation happens once models are capable enough. See [[product-as-organism]].

**Agents: three defining dimensions**
Aparna Chennapragada defines agents through three dimensions: (1) autonomy — a spectrum of delegation from copilot to fully autonomous; (2) complexity — multi-step goal-oriented tasks, not one-shot; (3) natural interaction — asynchronous, voice-capable, not just chat. The "agentic society" (Asha Sharma) is a world where the marginal cost of output approaches zero and exponential demand is met by agent proliferation. At Microsoft Azure, 15,000+ enterprise customers have deployed millions of agents.

**Successful AI company pattern (Asha Sharma)**
Three stages: (1) everyone becomes AI-fluent; (2) apply AI to existing processes and complete the P&L feedback loop; (3) use AI to inflect growth (better LTV, new categories, agentic workflows). Companies fail by doing AI for AI's sake, launching too many parallel projects without measurement, and not treating it as a real investment.

**Agents as the new software form factor (Bret Taylor)**
Bret Taylor at Sierra argues agents are "the new app" — the product form factor that defines the next era of software just as mobile apps defined the last. The key distinction from earlier software: agents accomplish jobs autonomously, making both the productivity gains and the ROI attribution self-evident. This is why outcomes-based pricing ("pay per resolution") is natural for agents but awkward for traditional SaaS. Taylor predicts the AI market will consolidate into three layers: (1) a handful of hyperscalers building foundation models (too CapEx-heavy for startups); (2) AI tooling companies (close to the sun, vulnerable to foundation model company competition); (3) applied AI / agent companies — the SaaS analog, with domain-specific moats and outcome-based business models. See [[outcomes-based-pricing]].

**The era of evals (Brendan Foody)**
Brendan Foody, CEO of Mercor, argues that the primary bottleneck to improving AI models is not more pre-training data but high-quality evals: "If the model is the product, then the eval is the PRD." Evals define what success looks like across every capability domain, power reinforcement learning from human/AI feedback, and serve as sales collateral. The market is shifting from crowdsourced low-skilled data labeling to sourcing credentialed domain experts (lawyers, doctors, engineers) who can write meaningful evals. The top 10% of contributors drive the majority of model improvement — making expert sourcing and assessment the core moat. See [[ai-evals]].

**Distribution platforms and AI (Brian Balfour)**
Brian Balfour predicts that the AI wave will follow the same platform cycle as previous technology shifts — and that ChatGPT is likely to become the next major distribution channel within 6–12 months. The moat being built: context and memory (the more you use ChatGPT, the better it knows you). The opening: a third-party agent platform allowing developers to build on top. Once that platform opens, the same gold rush dynamics that applied to Facebook in 2007 will apply — and companies that don't build on it risk ceding distribution to competitors. See [[distribution-platform-cycle]].

## Sources
- [[aishwarya-naresh-reganti-kiriti-badam]] — "80% of successful AI builders spend their time understanding workflows, not building models" (AI product development and the CC/CD lifecycle)
- [[alexander-embiricos]] — "Any capable agent should be a coding agent — human typing speed is the real bottleneck" (Agentic products and interaction design)
- [[alex-komoroske]] — "LLMs are magical duct tape — when execution is commoditized, taste is the differentiator" (AI strategy and product thinking)
- [[amjad-masad]] — "What if you made everyone a developer? What does that look like?" (Behind the product: Replit)
- [[anton-osika]] — "People love the product. That's the driver of the growth." (Building Lovable: $10M ARR in 60 days with 15 people)
- [[andrew-wilkinson]] — "It's like having the world's most reliable employee who costs $200 a month and works 24/7" (I've run 75+ businesses)
- [[aparna-chennapragada]] — "NLX is the new UX. Conversations have grammars, structures, UI elements — they're just invisible." (Microsoft CPO)
- [[asha-sharma]] — "Products as organisms just get better with more interactions. This is the new IP of every single company." (How 80,000 companies build with AI)
- [[bret-taylor]] — "The whole market is going to go towards agents. Agents are the new apps." (He saved OpenAI, invented the 'Like' button, and built Google Maps)
- [[brendan-foody]] — "If the model is the product, then the eval is the PRD." (Why experts writing AI evals is creating the fastest-growing companies in history)
- [[brian-balfour]] — "ChatGPT will be the next major distribution platform." (Why ChatGPT will be the next big growth channel)
- [[dan-shipper]] — "Context engineering is the skill. How you construct the context window determines 80% of the output quality." (How AI is changing the way we build products)
- [[chip-huyen]] — "Talk to users. Prepare better data. Write better prompts. That's what actually moves the needle." (AI engineering and the real bottlenecks)

**What actually improves AI apps (vs. what companies focus on)**
Chip Huyen distills the core mistake in AI product development: teams obsess over infrastructure (model choice, vector database selection, agentic framework adoption, staying current with AI news) while neglecting what actually moves the needle — talking to users, preparing better data, optimizing end-to-end workflows, writing better prompts, and building more reliable platforms. For RAG specifically, the biggest performance gains come from better data preparation (chunk sizing, metadata enrichment, hypothetical Q&A rewriting), not from database choice. For evals, the right question is coverage: do your evals reveal where the system is failing and guide what to fix? For AI tool adoption in organizations, productivity gains are highly heterogeneous — senior engineers often get the most benefit from coding agents because they use the tools most effectively.

**Post-training as the new battleground**
Chip Huyen explains why frontier labs are increasingly focused on post-training rather than pre-training: pre-training data has largely been exhausted (internet text), so differentiation now comes from RLHF, supervised fine-tuning, and verifiable reward training. The implication for AI product teams: fine-tuning a model for a specific domain can meaningfully improve performance — but it requires domain expert data creators and a clear evaluation framework.

---

**The AI-native company model (Dan Shipper / Every)**
[[dan-shipper]], CEO of Every, operates the most concrete example in the Lenny's catalog of what an AI-native company actually looks like. Every has 15 people and 5 products — a ratio that would be impossible without AI handling execution at scale. Shipper's key contributions to the AI product conversation:

- **Context engineering**: His term for the practice of carefully constructing the context window you give an AI model — selecting the right documents, examples, and constraints. As models get more capable, context engineering becomes the primary skill for getting great outputs. It's distinct from prompt engineering (one-shot instructions) because it operates at the system and session level.
- **The head of AI operations role**: Shipper argues every AI-forward company needs someone who maps company workflows, identifies where AI applies, and redesigns the remaining human work. This is an organizational design role, not a technical one. See [[ai-operations-role]].
- **AGI as leash length**: Practical definition: how long a task can you give an AI autonomously before it makes a mistake you care about? Today's models handle well-defined 30-minute tasks reliably. AGI is when the leash is effectively infinite.
- **Claude Code for non-coders**: Shipper is an enthusiastic practitioner of Claude Code (Anthropic's coding agent) and argues it's not primarily an engineer's tool — it's a tool for anyone who can describe precisely what to build. The bottleneck is not coding; it's clarity of thought.

**The AI-native enterprise: Block's Goose model (Dhanji R. Prasanna)**
Dhanji R. Prasanna ([[dhanji-r-prasanna]]), CTO of Block, argues that the AI-native enterprise is not one that uses AI tools but one built around AI as a first-class operating layer. Block's internal agent platform, **Goose**, is an open-source AI agent designed for engineering workflows — not just code generation but running tests, debugging, deploying, and interacting with internal systems. Block's approach: rather than each team building their own AI integrations, Goose becomes a shared agent substrate. Extensions allow teams to add new capabilities without duplicating infrastructure.

Prasanna's key insight on enterprise AI adoption: the bottleneck is not model capability — it's the **context gap**. AI agents without context about your systems, codebase, and organizational patterns are only marginally useful. The investments that pay off are those that give agents the right context: MCP (Model Context Protocol) servers that expose internal tools, documentation that's agent-readable, and code architectures that agents can navigate.

His org structure observation: Block uses a **functional org** (not a divisional or matrix) — grouping by discipline (all engineers together, all designers together) rather than by product team. In an AI-accelerated world, this enables faster skills transfer, cleaner AI tooling adoption, and avoids the silo problems that slow AI integration in matrix orgs.

**Spatial intelligence as the missing AI dimension (Dr. Fei-Fei Li)**
Dr. Fei-Fei Li ([[dr-fei-fei-li]]) identifies a foundational gap in current AI products: language models cover only one dimension of human intelligence. The spatial dimension — 3D reasoning, object manipulation, environmental navigation — is largely absent. Her company World Labs is building world models: foundation models that generate navigable, interactive 3D worlds from text or image prompts.

For product builders, the near-term implication is sector-specific: world models will matter most for robotics, VFX/virtual production, game development, and scientific simulation. But Li's broader argument is that spatial intelligence AI will augment humans the way language models augment language work — and that current world model demos (which "look like toys") should be watched carefully, as that pattern has preceded every major AI capability jump. See [[world-models]].

## See Also
- [[ai-operations-role]]
- [[context-engineering]]
- [[continuous-calibration-continuous-development]]
- [[agency-control-tradeoff-ladder]]
- [[ai-non-determinism]]
- [[taste-as-competitive-advantage]]
- [[ai-computer-interfaces]]
- [[jevons-paradox-software]]
- [[minimum-lovable-product]]
- [[lazy-leadership]]
- [[nlx-natural-language-experience]]
- [[product-as-organism]]
- [[outcomes-based-pricing]]
- [[distribution-platform-cycle]]
- [[ai-evals]]
- [[chip-huyen]]
- [[world-models]]
- [[dhanji-r-prasanna]]
- [[dr-fei-fei-li]]
