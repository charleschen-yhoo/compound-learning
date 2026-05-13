---
id: "074"
title: "Action Required Emails iOS — Stats Sig Lift in Opens and CTR"
date: 2024-11-01
source: "Read Write Search Squad MPU Decks, Nov 2024"
themes: [engagement-features, reading, mobile, email-classification]
confidence: medium
goal: "engagement"
---

## Hypothesis
By surfacing required actions for users to take on emails in the inbox list for Yahoo Mail Openers, we expect to increase our quality open per opener metric by 1% because we are reducing the time it takes for a user to take actions on appropriate emails by surfacing these actions one level higher in the funnel.

Feature leverages important email decos and Mandalore's dynamic action prediction model to add decorations on the inbox level (e.g., Reply, Move, Archive). Works with TLDR quick tap actions.

## Test Design
- **Platform**: iOS
- **Bucket**: 8%, 1% MDE, 2 weeks
- **Variants**: T1 (pink), T2 (orange), T3 (green)
- **Metrics**: Quality open per opener (primary), opens, CTR
- **Status**: In Experiment — iterating

## Outcome
**Primary Metric (quality open per opener): non-stats-sig positive**
- T2 orange: +0.35%
- T3 green: +0.27%
- T1 pink: +0.01%

**Stats-sig lift in # of opens:**
- T2 orange: **+14%**
- T1 pink: +11%
- T3 green: +4%

**Stats-sig lift in CTR** (control baseline: 0.38%):
- T2 orange: **+22%** (→ 0.46%)
- T1 pink: +18% (→ 0.45%)
- T3 green: +7% (→ 0.41%)

**Guardrails:**
- No stats-sig change in % Open 7+ in 7 days
- No stats difference in number of eligible emails per cohort
- All other Mail guardrails neutral/within normal range

**Next steps:** Iterate with T2 (orange) variant and update criteria for what constitutes an action-required email.

## Nuance
Orange consistently outperforms across all metrics (opens, CTR, and even the non-sig primary metric). The color hierarchy — orange > pink > green — maps to attention urgency, which makes intuitive sense for "action required" flags.

The gap between strong secondary metrics (opens +14%, CTR +22%) and non-significant primary metric (+0.35%) suggests the model correctly identifies emails users will open, but the downstream quality action (the extra step from open to meaningful engagement) isn't yet triggered reliably. The criteria for "action required" may need tightening — casting too wide a net dilutes the signal.

This is a "reading" enhancement that surfaces actionability at the inbox level, similar in spirit to Tidy Inbox [037] but at the individual email level. It also connects to the TLDR quick tap actions (Haven), creating a pipeline: see action flag → tap to open → see TLDR summary → take quick action.
