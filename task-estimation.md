# Task Estimation in Scrum

> **TL;DR:** Estimates are always uncertain. Use them as a tool for planning and discussion, not as deadlines or performance targets. The goal is to improve over time, not to be perfect from the start.

---

## Why Estimation Matters

Poor estimates are one of the most common reasons projects fail. In one real project involving AI-driven NPCs for a video game, the AI component was left too late — by the deadline, the NPCs barely worked. The task had been underestimated, work started late, and there was no time to recover. In a startup with 20 engineers, this kind of delay leads to missed releases, rushed features, and bugs in production. When done poorly, estimation creates false confidence and pressure that makes outcomes *worse*.

---

## Why Estimates Go Wrong

The diagram below summarises the most common structural reasons behind this.

![Summary of reasons why planning-based estimation fails](images/planning-based-estimation-doesn't-work.png)
*Source: Urs Enzler, Planet Geek (2024) — [(Mis)estimation – why estimates tend to be wrong](https://www.planetgeek.ch/2024/02/07/misestimation-why-estimation-does-not-work/)*

A particularly clear illustration of the gap between plans and reality is the following diagram, which shows how what teams plan at the start rarely matches what actually gets delivered.

![Plan vs. reality in software projects](images/plan_vs_reality.png)
*Source: Urs Enzler, Planet Geek (2024) — [(Mis)estimation – why estimates tend to be wrong](https://www.planetgeek.ch/2024/02/07/misestimation-why-estimation-does-not-work/)*

**Common causes:**

- **Optimism bias:** developers estimate the happy path — no blockers, no unclear requirements, no integration surprises. Daigle (DEPT Agency) describes this as one of the most persistent problems in engineering teams: complications always appear, and they always take time [(Daigle, DEPT Agency)](https://engineering.deptagency.com/why-software-development-estimates-are-so-often-wrong).
- **Estimating too early:** estimates are locked in at the start of a project, when the team knows the *least* about the work. Initial estimates can easily end up 2–4 times too low.
- **Hidden complexity compounds:** Enzler found that 100 tasks, each with only 1–2% extra integration work, can add 70–200 unplanned days to a project — a number no one would have predicted at the start [(Enzler, Planet Geek)](https://www.planetgeek.ch/2024/02/07/misestimation-why-estimation-does-not-work/).
- **Anchoring bias:** whoever speaks first sets an invisible ceiling. Other team members adjust toward that number rather than thinking independently — a pattern Agile Seekers found repeated across teams regardless of experience level [(Agile Seekers)](https://agileseekers.com/blog/cognitive-biases-that-ruin-sprint-planning-and-how-to-avoid-them).
- **Velocity used as a performance metric:** when teams are measured by velocity, they inflate estimates to look more productive. Walsh at Axify describes this as the point where the data becomes completely unreliable [(Walsh, Axify)](https://axify.io/blog/story-points).

---

## The Estimation Process in Practice

![Limitations of story points in software development](images/limitations%20of%20story%20points%20in%20software%20development.webp)
*Source: Alexandre Walsh, Axify — [Why Story Points Don't Matter and What to Use Instead](https://axify.io/blog/story-points)*

---

## Good Practices to Follow

- **Prefer relative complexity over hours.** Hours become deadlines. Story points avoid false precision — but only if the team uses reference stories to anchor the scale.
- **Estimate as a team, at the same time.** When one person dominates, the result reflects one opinion. Disagreement is often where the most valuable discussion happens.
- **Break down anything that feels uncertain.** If a task cannot be estimated with confidence, it is too big or too vague.
- **Update estimates when scope changes.** Silently hoping to catch up is how sprints collapse.
- **Review actual results in retrospectives.** Consistent estimation errors in the same direction are a process problem, not bad luck.

---

## At a Glance

| Good practice | Anti-pattern |
|---|---|
| Estimate together as a team | One person estimates for everyone |
| Use relative sizing with reference examples | Invent a scale with no shared anchor |
| Discuss disagreements instead of averaging | Average outliers away to move faster |
| Break stories down before estimating | Accept vague, unrefined tasks into planning |
| Track velocity over multiple sprints | Start from scratch each sprint |
| Treat estimates as forecasts | Treat estimates as deadlines or commitments |
| Revise estimates when scope changes | Hold people to estimates after requirements change |

> **Common failure mode:** management treats estimates as promises, so engineers pad numbers defensively. Be transparent: estimates are forecasts, not contracts.

---

## Common Themes Across Sources

After reviewing the five references, several themes came up consistently — not as theory, but as things practitioners had experienced and struggled with:

- **Estimates always become deadlines, unless you actively prevent it.** Every source describes the same pattern: a rough estimate gets repeated up the chain and arrives at the client as a commitment. Engineers then feel accountable for a number that was never meant to be precise.
- **The psychological pressures are harder to fix than the process.** Optimism, anchoring, and fear of looking slow distort estimates even in teams with good intentions. Multiple sources point out that awareness alone is not enough — the environment has to make honest estimation safe.
- **Looking back is the only way to get better.** Every source that discusses improvement points to retrospectives and comparing estimates to actuals. Teams that skip this step have no signal for whether they are improving or just repeating the same patterns.

---

## Quick Reference: Estimation Template

Use this template during sprint planning sessions:

1. **Task name and description**: Clear, specific, and refined
2. **Relative complexity**: Compared to similar past tasks (reference story)
3. **Rough duration estimate**: "Half a day", "2-3 days", "uncertain - needs spike"
4. **Risk factors**: What could make this take longer?
5. **Dependencies**: Does this task block or depend on others?
6. **Confidence level**: High / Medium / Low

---

## References

1. [Why software development estimates are so often wrong](https://engineering.deptagency.com/why-software-development-estimates-are-so-often-wrong) by Matt Daigle, DEPT Agency
2. [How to Fix Story Point Estimation](https://www.humanizingwork.com/how-to-fix-story-point-estimation/) by Peter Green, Humanizing Work
3. [Cognitive Biases That Ruin Sprint Planning and How To Avoid Them](https://agileseekers.com/blog/cognitive-biases-that-ruin-sprint-planning-and-how-to-avoid-them) by Agile Seekers
4. [Why Story Points Don't Matter and What to Use Instead](https://axify.io/blog/story-points) by Alexandre Walsh, Axify
5. [(Mis)estimation – why estimates tend to be wrong](https://www.planetgeek.ch/2024/02/07/misestimation-why-estimation-does-not-work/) by Urs Enzler, Planet Geek

