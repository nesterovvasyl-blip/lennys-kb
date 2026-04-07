---
aliases: [spatial intelligence, 3D world generation, world model AI]
guests: [dr-fei-fei-li]
---

# World Models

> Foundation models that can generate navigable, interactive, 3D worlds from text or image prompts — the spatial intelligence dimension of AI that language models don't provide.

## Content

The concept of world models, articulated most directly by Dr. Fei-Fei Li ([[dr-fei-fei-li]]) at World Labs, addresses a fundamental gap in current AI: language models have achieved a breakthrough in the *language* dimension of intelligence, but human intelligence has a second major dimension that AI has barely touched — spatial intelligence.

### The Core Argument

Humans are deeply visual, spatial animals. We interact with the world at the object level, in 3D, through movement and manipulation. A child can count the chairs in a room by watching a video. A physicist can derive equations by observing celestial body motion. A surgeon navigates complex 3D geometry without thinking about it.

Current AI cannot do these things. Language models trained on text and images are powerful pattern-matchers in the language domain. They have limited 3D spatial reasoning, no understanding of physical dynamics, and no ability to generate interactive environments.

World models fill this gap. A world model is a foundation model that:
- Understands 3D structure from 2D observations
- Can generate navigable, interactive 3D worlds from prompts
- Models physical dynamics and object interactions
- Enables spatial reasoning at scale

### The "Golden Recipe" Parallel

Dr. Fei-Fei Li draws an explicit parallel to the 2012 ImageNet breakthrough that sparked the deep learning revolution. That breakthrough required three ingredients: large-scale labeled data (ImageNet), neural networks, and GPUs. The combination produced the modern AI era.

World models require an analogous convergence — large-scale 3D data, new architectures capable of spatial reasoning, and sufficient compute. Her argument: we are approaching that convergence now, and the resulting capability jump could be as significant as 2012.

### Applications

**Near-term:**
- **VFX and virtual production**: World Labs demonstrated 40x production time reduction in film/TV content creation
- **Game development**: Generative 3D worlds rather than hand-crafted environments
- **Architectural and product visualization**: Interactive 3D prototypes from natural language descriptions

**Longer-term:**
- **Robotics**: Training data for robots requires 3D world simulation, not just text or image data. The "bitter lesson" (simpler models + more data always win) applies to robotics differently than to language — robots need action-grounded spatial data.
- **Scientific discovery**: Simulating physical systems for research in materials science, drug discovery, climate modeling
- **Human augmentation**: Spatial intelligence tools that extend how humans perceive and interact with physical environments

### Not the Same as Language Models

A common misconception is that more capable language models will eventually develop spatial intelligence. Li's view: spatial intelligence is a distinct capability dimension that requires distinct architectures and training approaches. The same way you can't derive the equations of motion by reading physics textbooks (but you can by observing physical systems), language-only training has fundamental limits for spatial reasoning.

### The "Looks Like a Toy" Warning

Li observes that world models currently look like playful 3D world generators — impressive demos, not yet transformative products. She notes this is exactly what ChatGPT looked like in 2022. The pattern of "looks like a toy → becomes civilizational infrastructure" has repeated across every major technology wave. Her advice: don't dismiss things that look like toys.

## Sources
- [[dr-fei-fei-li]] — "The Godmother of AI on jobs, robots & why world models are next" (Lenny's Podcast, 2025-11-16)

## See Also
- [[ai-products]]
- [[ai-non-determinism]]
- [[dr-fei-fei-li]]
