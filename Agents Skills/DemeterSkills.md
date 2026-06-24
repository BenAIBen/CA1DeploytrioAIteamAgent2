---
name: forecast-winter-capacity
description: Use when basket composition, seasonal value perception, or winter capacity planning needs to be modeled ahead of a visible customer-facing dip. Triggers on "what does the basket look like for the next 8 weeks", "build the winter capacity gap report", "are we about to hit a value-perception dip", "should we launch a winter-specific tier", "check basket composition against last year".
owner: Demeter Voss, Scientist (demand forecasting and supply chain lead)
created: 2026-06-23
---

# Forecast Winter Capacity

## When to use
- A seasonal report or capacity plan is being built and basket composition data exists or can be gathered.
- Someone is proposing a winter promotion, tier, or pricing change and needs to check it against real basket diversity first.
- Subscriber growth or waitlist conversion is being discussed and the supply side has not been checked.
- A value-perception dip is suspected but no one has dated exactly when it starts.
- Do not use when the question is about why subscribers are already churning (that is Ceres's job) or how to convert a waitlist segment (that is Osiris's job); Demeter only establishes the supply and capacity facts those two build on.

## Inputs needed
- Weekly or monthly basket logs (SKU count, price per item, basket value): required. If missing, ask: "Can you share the basket logs or production data for the period in question?"
- Production calendar (planted or growing crops, expected yield, SKU contribution by month): required. If missing, ask: "What does the production calendar look like for the months in question?"
- Subscriber cohort sizes by sign-up month: optional, needed only to model capacity ceilings. If missing, ask: "Do you have subscriber counts by sign-up month, or should I model basket composition only?"
- Prior-year basket data for the same period: optional. If missing, proceed without it and flag the gap in the output.

## Steps
1. Aggregate the basket logs to a monthly view: average SKU count, average price per item, average basket value.
2. Calculate month-over-month percent change in basket value to find the steepest drop, not just the lowest point.
3. Name the exact week diversity crosses below a threshold a customer would notice, using the SKU count, not the calendar label.
4. Classify the dip as a production problem, a packaging or timing problem, or a genuine shortfall; state which, in one line.
5. If cohort data is available, calculate the capacity ceiling: total estimated churned seats versus the available conversion pool (such as a waitlist), and state the percentage gap.
6. Write a short verdict: is this a season to smooth, or does it justify a permanent winter-specific tier.
7. Close with a numbered handoff list naming exactly what the next agent (Ceres or Osiris) receives and should do with it.

## Output contract
- Length: half a page to one page.
- Format: opens with a one-line provocation in Demeter's voice, then a monthly table, then a cliff table (transition, percent change), then 2 to 4 short paragraphs, then a numbered handoff list.
- Must include: the dated cliff week, the production-vs-shortfall classification, the capacity ceiling number if cohort data exists, a handoff list.
- Must not include: hedged language, generic seasonal commentary without a number attached, chart descriptions in prose, padding or reassurance.
- Business writing: concise, declarative sentences, no jargon without a number attached.
- Skeleton: