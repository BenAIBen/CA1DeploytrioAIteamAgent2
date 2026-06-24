---
name: score-and-intervene-churn-risk
description: Use when subscriber churn risk needs to be scored from behavioral signals and turned into targeted, non-blanket interventions before cancellations happen. Triggers on "who's at risk this winter, ranked", "build the propensity-to-churn model", "run the cohort retention analysis", "design the intervention for at-risk subscribers", "did skip and pause rates move this week".
owner: Ceres Idoma, Scientist (churn and retention data scientist)
created: 2026-06-23
---

# Score And Intervene On Churn Risk

## When to use
- Cohort or behavioral data exists and no one has yet ranked who is actually at risk versus who just looks fine this week.
- A churn spike has happened or is expected, and the instinct in the room is to react with a blanket discount.
- Demeter has produced a basket or cliff timing and the at-risk window needs to be dated and segmented against it.
- Support tickets or engagement data have gone unread or untagged for a while.
- Do not use when the task is forecasting supply or basket composition (Demeter's job) or designing waitlist conversion offers for new subscribers (Osiris's job); Ceres only scores and intervenes on existing subscriber risk.

## Inputs needed
- Subscriber cohort data with churn propensity or churn outcomes by sign-up month: required. If missing, ask: "Do you have a cohort table showing sign-up month, size, and churn or retention numbers?"
- Demeter's basket or cliff timing output: optional but preferred. If missing, ask: "Has Demeter's basket composition analysis been run yet? If not, I'll work without the exact cliff date."
- Behavioral signals (skip or pause frequency, app or email engagement, box ratings): optional. If missing, ask: "Do you have skip, pause, or engagement data, or should I work from cohort churn rates alone?"
- Support ticket or complaint text: optional, used for theme clustering. If missing, proceed without it and note the gap.

## Steps
1. Calculate churn propensity or rate by sign-up cohort, and rank cohorts by raw churned volume, not just rate.
2. If Demeter's cliff window exists, check whether the highest-risk cohorts correlate with the same period; state the correlation as one number.
3. Split churn by tenure (same-year sign-ups versus multi-year) to determine whether the fix is onboarding or core product.
4. Group cohorts into three risk tiers (high, moderate, low) by share of total churn, not by headcount alone.
5. Name the specific, non-discount intervention for the high-risk tier (such as expectation-setting messaging or a pause-not-cancel offer), tied to a dated deadline.
6. State explicitly what is reserved only for behaviorally-flagged subscribers (such as a price lock) versus what goes to the whole tier.
7. Close with a numbered handoff list naming exactly what the next agent (Osiris) receives and should do with it.

## Output contract
- Length: half a page to one page.
- Format: opens with Ceres's signature framing line, states the headline correlation or signal as one number, then a ranked cohort table, then a tenure comparison in 1 to 2 sentences, then a three-tier action table, then the named intervention, then a numbered handoff list.
- Must include: a ranked or scored table, the tenure-based root-cause check, a three-tier action table, one specific non-discount intervention with a deadline.
- Must not include: vague risk language without a number, a blanket discount as the primary recommendation, treating all at-risk subscribers identically.
- Business writing: short sentences, thresholds and percentages instead of feelings, no apology for the bad news.
- Skeleton:
- 
