---
guest: Karina Nguyen
role: AI Researcher at OpenAI (formerly Anthropic)
episode: "OpenAI researcher on why soft skills are the future of work | Karina Nguyen"
date: 2025-02-09
topics: [ai, model-training, product-development, future-of-work, soft-skills, openai, anthropic]
---

# Karina Nguyen

> AI researcher at OpenAI who helped build Canvas, Tasks, and the o1 reasoning model; previously at Anthropic where she led post-training and evaluation for Claude 3 and built the 100K context window file upload feature; also a former engineer at the New York Times and designer at Dropbox and Square.

## Content

Karina Nguyen has one of the most unusual trajectories in AI: she went from frontend engineering to design to AI research, with stints at Square, Dropbox, the New York Times, Anthropic, and OpenAI. She made the switch from engineering to research at Anthropic after realizing that Claude was becoming capable enough at coding that research would matter more than her current skillset. At OpenAI, she joined about eight months before this episode and played a core role in building Canvas (OpenAI's collaborative document/code editing interface), Tasks (their first async agent feature), and the o1 reasoning model. She is now also managing and mentoring on her team.

Her episode is one of the clearest inside views of how AI products are actually built at frontier labs, combined with forward-looking speculation on what skills will matter most as AI gets smarter.

### Key Ideas

- **Model Training is an Art, Not a Science**: Karina describes debugging models as similar to debugging software — you trace back to the training data and identify why specific behaviors emerged. Key example: when Claude 3 was taught it didn't have a physical body (for safety), this conflicted with tool-use training (like setting alarms), causing the model to confusingly refuse some tasks. Data quality is the most important lever in model training.

- **Synthetic Data for Product Features**: Karina explains how Canvas and Tasks were primarily built using synthetically generated training data — not human-labeled examples. The process: (1) identify 2-3 core behaviors you want the model to have; (2) use o1 to generate diverse synthetic conversations representing those behaviors; (3) build deterministic evals to measure pass/fail; (4) iterate. This made Canvas possible in 4-5 months from zero to one. The key advantage of synthetic data: cheap, scalable, and can be shifted rapidly based on user feedback post-launch.

- **Evals as the New PRD**: Product development for AI features increasingly means defining what "correct" looks like (evals) rather than writing specifications for human engineers to implement. Product managers and model designers at OpenAI learn to write spreadsheets with columns for current behavior, ideal behavior, and why — which serve as both evaluation data and potential training data. The intuition: if you can't define correct, you can't build or improve the feature.

- **Prompting as Product Prototyping**: Before writing a line of training code, Karina uses prompting to prototype new feature ideas. She gives the example of building a 100K context window demo by simply prompting Claude in a browser — the user enthusiasm demonstrated product-market fit that justified the full build. This is the new "scratch an itch" prototyping paradigm: prompting is now a design tool.

- **The No Data Wall Thesis**: The common concern about AI running out of training data assumes only pre-training (internet-scale text) matters. But o1 and its successors are trained primarily through post-training reinforcement learning on tasks — and there's an essentially infinite space of tasks to teach. The bottleneck has shifted from "data about the world" to "useful tasks and correct evaluations."

- **Soft Skills as the Durable Advantage**: Karina argues that creative thinking, aesthetic taste, management, empathy, and collaboration are the skills that will remain distinctly human the longest. AI research progress is itself bottlenecked by research management — the ability to prioritize experiments, allocate compute with conviction, and organize teams for maximum output. The hard skills (coding, writing, analysis) are being commoditized; the soft skills (which are actually very hard) are the moat.

- **Anthropic vs. OpenAI Cultural Differences**: More similar than different, but two distinctions: Anthropic has deeper craft and care around model character and personality — Claude's personality reflects the detailed curation of its creators. OpenAI has more "creative product freedom" and is more bottom-up/risk-taking in product innovation; Anthropic has more focused, hardcore prioritization. Both reflect the cultures of their founding teams.

- **Form Follows Function in AI Products**: Karina emphasizes that the power of features like Canvas and 100K context isn't the raw technical capability — it's finding the right form factor that makes the capability feel natural. File uploads were natural; an infinite scroll chat with 100K context would have been confusing. The hard design question for the next era: how do you make async agentic AI feel trustworthy and natural when it operates in the background?

### Actionable Advice

- When building AI features, start by defining 2-3 core behaviors in concrete pass/fail terms — this is your eval and likely your training signal.
- Prototype with prompting before committing to training — prompting reveals product-market fit quickly and cheaply.
- Build for the model capability that will exist when your product launches, not today's model — "the right product ideas will just work" as models improve.
- Focus skill development on creativity, taste, listening, and management — the things LLMs are still genuinely bad at.
- Use AI as a personalized learning tool: ask it to customize curricula to your learning style, then test your understanding by explaining back to the AI.

### Notable Quotes

> "When I first came to Anthropic I was like, 'Oh my God, I really love front-end engineering.' And then the reason why I switched to research is because I realized, 'Oh my God, Claude is getting better at front-end.'"

> "The cost of reasoning and intelligence is drastically going down."

> "I think it's actually really, really hard to teach the model how to be aesthetic or do really good visual design or how to be extremely creative in the way they write."

> "We went from personal computers to personal models basically."

## Sources

- [[karina-nguyen]] — "OpenAI researcher on why soft skills are the future of work | Karina Nguyen"

## See Also

- [[ai-evals]]
- [[ai-training-data]]
- [[context-engineering]]
- [[world-models]]
- [[future-of-work]]
