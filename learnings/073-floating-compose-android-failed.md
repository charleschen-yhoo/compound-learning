---
id: "073"
title: "Floating Compose Android — Failed"
date: 2024-11-01
source: "Read Write Search Squad MPU Decks, Nov 2024"
themes: [engagement-features, writing, mobile, failed-experiment]
confidence: high
goal: "engagement"
---

## Hypothesis
By providing a floating compose button in the bottom right corner of the inbox for Compose users, we expect to have a 2% lift on average message send per DAU because we are reducing friction in message composes.

## Test Design
- **Platform**: Android
- **Bucket**: 10%, 2% MDE, 3 weeks
- **Metric**: New compose sends, compose-to-send conversion
- **Status**: Terminated — do not ship

## Outcome
- **New Compose Sends: no stats sig lift in any of the variants**
- CTR: Variant 3 had the highest at +1%
- **Compose to Send Conversion: Control had the highest conversion %** — the FAB generated more compose taps but fewer completions
- No negative impact to sends (helpful data point for 2025 mobile redesign)

**Key learnings:**
- Novelty shaken off: ran for 3 weeks, looked at last 2 weeks of data — current experience still outperformed
- Variant 3's higher CTR was likely due to placement and size of the new compose button, but this didn't translate to overall send lift because "it's hard to foster users' intent to compose"
- **Confidence to focus on compose-to-send conversion rather than top of funnel**

## Nuance
This is a more nuanced failure than "nothing happened." The FAB successfully got more users to *tap* compose (Variant 3 +1% CTR), but those incremental taps didn't convert to sends — control had the highest compose-to-send conversion. This means the FAB attracted low-intent taps: users who were curious about the button but didn't actually want to write an email.

The team's takeaway is strategically important: for Q1 2025, focus shifts to **smart replies, auto-complete, and AI compose** — features that help users who have already started composing to finish, rather than features that try to get more users to start.

This pairs with Draft Nudges (Desktop, upcoming): another approach to the compose-to-send conversion problem, targeting users who started but abandoned drafts.
