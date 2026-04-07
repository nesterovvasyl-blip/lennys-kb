---
aliases: [three-eras-internet-products, curation-to-generation]
guests: [gustav-söderström]
---

# Curation → Recommendation → Generation

> The three eras of internet product development: human curation, algorithmic recommendation, and generative AI — each removing a layer of friction between users and the content or experience they want.

## Content

Framework articulated by [[gustav-söderström]], CPTO of Spotify, to describe how internet products have evolved in how they surface value to users.

**Era 1: Curation**
Human editors, curators, and experts decided what content was shown and in what order. Examples: editorial staff picking homepage stories, playlist editors selecting "New Music Friday" tracks, Tumblr staff picks. Curation is high-quality but doesn't scale — the number of curators constrains how personalized or comprehensive the output can be. It also embeds the curators' taste and biases as defaults for all users.

**Era 2: Recommendation**
Machine learning systems replaced (or supplemented) human curation by analyzing behavioral data — what users clicked, listened to, bought, or rated — and using it to predict what each individual user wants next. Examples: Netflix's movie recommendations, Spotify's Discover Weekly, Amazon's "customers also bought." This scaled curation to billions of users, but created new problems: the "taste bubble" (recommendations optimize for your past preferences, not your future potential interests) and cold-start failures (no data means no recommendations for new users).

**Era 3: Generation**
ML systems don't just recommend existing content — they generate new content, new experiences, or new interfaces from a prompt or context. Examples: AI writing assistants, image generators, v0 generating UI from a description, Spotify generating personalized radio commentary or playlist introductions. The key shift: the output space is no longer constrained to existing content; the model creates what doesn't yet exist in response to the specific need. This is the current era, beginning around 2022-2023.

**Implications for product design**:
- Each era changes the design of the product surface. Curation requires editorial tools. Recommendation requires feedback signals (ratings, implicit signals) and surfacing mechanisms (homepages, feeds). Generation requires prompting interfaces, output refinement mechanisms, and escape hatches (see [[fault-tolerant-ui]]).
- Each era also changes the metric that matters most. Curation: editorial quality. Recommendation: click-through rate, watch rate, session length. Generation: task completion, output quality, user satisfaction with generated content.
- The transition between eras creates tension: teams invested in the previous era's approach resist the shift.

**Spotify's homepage as a case study**: Söderström describes the homepage redesign as navigating the tension between "recall mode" (give me exactly what I've been listening to — the recommendation era) and "discovery mode" (show me what I'd love but haven't encountered — the challenge of generation). The homepage must balance both, and the right balance isn't static — it depends on user context (commute vs. workout vs. focus work).

**The "taste bubble" problem**: The deepest unsolved challenge in the recommendation era is that optimization for revealed preferences reinforces existing taste rather than expanding it. A user who listens mostly to jazz gets more jazz. The generation era offers a partial solution: generated content can be explicitly designed to be adjacent to but different from existing preferences, expanding the taste bubble rather than reinforcing it.

## Sources
- [[gustav-söderström]] — "How Spotify builds product" (2023)

## See Also
- [[gustav-söderström]]
- [[fault-tolerant-ui]]
- [[ai-products]]
