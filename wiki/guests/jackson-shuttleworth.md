---
guest: Jackson Shuttleworth
role: Group PM, Retention Team, Duolingo
episode: "Behind the product: Duolingo streaks"
date: 2024-12-15
topics: [retention, growth, engagement, experimentation, gamification, metrics, streaks]
---
# Jackson Shuttleworth
> Group PM at Duolingo leading the retention team — the steward of streaks, Duolingo's single most impactful feature, which he and his team have improved through 600+ experiments over four years.

## Content

Jackson Shuttleworth is a Group Product Manager at Duolingo who leads the retention team. He oversees the streak feature — Duolingo's mechanism for tracking consecutive days of app use — which he characterizes as the single biggest growth lever in the product after the lessons themselves. He joined Duolingo shortly after a pivotal experiment (XP-based → lesson-based streak) that permanently changed the company's retention trajectory. Since then, his team has run over 600 experiments on the streak feature, averaging one every other day.

Duolingo is a $14B company at time of recording, having doubled in market cap over the six preceding months. Over 9 million users have a year-long-plus streak — effectively a city of daily language learners.

### Key Ideas

- **The streak's superpower**: Streaks are not just a retention feature in isolation — they are an enabler for other features (notifications, goal-setting, subscription pitches) because users who care about their streak are already activated. Duolingo's primary growth North Star is DAUs (daily active users), and the metric most closely correlated with DAU growth is CURR (current user retention rate — the rate at which non-new users return tomorrow). The streak is the best single driver of CURR.

- **Unit of use matters**: The XP-based streak required hitting a custom XP threshold, which caused users to lose streaks even on days they completed lessons. The shift to "complete one lesson = extend streak" caused a massive DAU jump. But going further (one exercise extends the streak) was tried and failed — it attracted the wrong users and diluted the meaning of the feature. The lesson: the streak unit must match the *meaningful* unit of use.

- **Zero-to-seven critical window**: Retention curves at Duolingo show that loss aversion (the psychological reluctance to break the streak) kicks in at day 7. Days 1–7 show sharply improving retention with each additional day of streak; after day 7 the improvement flattens. As a result, the team runs disproportionate experiments on getting users from zero to seven days.

- **Goal-setting as commitment device**: Adding a "streak goal" screen that told users they were X times more likely to finish their course with a 30-day streak was a massive win. Even more interesting: adding an opt-out button (letting users decline the 30-day goal) was also a big win. The act of intentionally committing (or consciously declining) created psychological stakes that improved retention — even though the commitment screen had zero downstream effect on streak mechanics.

- **Copy testing at scale**: Duolingo's infrastructure for copy testing allows rapid low-cost experimentation. Changing the goal screen CTA from "Continue" to "Commit To My Goal" was a top-three CURR win that drove ~10,000 incremental DAUs. The lesson: companies with the user base to run copy tests should do so constantly. The lifting is cheap; the wins can be enormous.

- **Ship neutral experiments cautiously**: About half of Duolingo's experiments lose. For neutral experiments, the default is to kill, not ship — adding UI elements even with zero measured effect increases cognitive load and creates future debt. The exception is when a neutral experiment is a necessary platform to enable the next set of positive experiments.

- **Don't ship wins that compromise core spaces**: Duolingo once ran a winning experiment adding XP counters to the in-lesson experience — and then decided not to ship it. The lesson screen is the most sacred space in the product (where learning actually happens); adding gamification elements to it came with a long-term strategy cost that wasn't worth a short-term engagement win.

- **Clarity over delight (at first)**: Duolingo's streak flame iconography is powerful for experienced users, but new users in some cultural contexts (e.g., India research) didn't understand the metaphor. The team evolved the design to lead with the number (an odometer animation ticking up) rather than the flame. Form should follow function; clarity at day one is more important than delight.

### Actionable Advice

- Identify the meaningful unit of use for your app and make your streak track *that* unit — not a harder or easier version.
- Run disproportionate experiments on the first 7 days of streak (or your equivalent critical activation window). Loss aversion, once active, does most of the work.
- Test copy constantly if you have the user base. The cheapest wins often come from words, not features.
- For any feature, ask: is this a local maximum? Periodically throw away accumulated UI optimizations and rebuild simpler — it's the only way to escape local maxima.

### Notable Quotes

> "We've run over 600 experiments on streaks in four years. Every other day. They range from changing how the mechanic works to swapping one string with another."

> "We shut down about half our experiments. Half of them lose. We still learn a ton from running them."

> "Say 'Commit To My Goal' instead of 'Continue' — that single copy change was a top-three CURR win for us."

> "Luis grant me the serenity to accept the flexibility I need, the courage to reach perfection when I can, and the wisdom to celebrate regardless." (The Duolingo Streak Serenity Prayer, embroidered and gifted to Jackson by his co-lead)

## Sources
- [[jackson-shuttleworth]] — "Behind the product: Duolingo streaks"

## See Also
- [[experimentation-culture]]
- [[gamification-three-pillars]]
- [[retention]]
- [[engagement]]
