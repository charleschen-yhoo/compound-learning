---
id: "072"
title: "Emoji Reactions Android — +2.97% Replies Lift, No Cannibalization"
date: 2024-11-01
source: "Read Write Search Squad MPU Decks, Sept-Nov 2024"
themes: [engagement-features, writing, mobile, reactions]
confidence: high
goal: "engagement"
---

## Hypothesis
Yahoo Mail DAUs reply/reply-all more (iOS 6%, Android 4%) than they compose fresh emails (iOS 4%, Android 3%). Users currently take 3 steps from message open to reply (tap reply, add content, press Send). By providing emoji reactions as a way to reply/respond to emails from people, we expect to increase Replies/Reply-Alls per Opener by 2%.

## Test Design
- **Platform**: Android
- **Bucket**: 8%, 2% MDE, 2 weeks
- **Metric**: Replies/reply-all per user (target: 2% lift)
- **Status**: GA approved → GA planned in 7.55 (12/06)

## Outcome
- **+2.97% stats sig lift in replies/reply-all per user** (exceeded 2% target)
- No significant impact to Mail guardrails
- **+1% non-stats-sig lift in Sends per DAU**
- **-0.48% non-stats-sig decrease in Quality Opens per Opener**
- **No cannibalization on toolbar replies and quick replies** — this is additive, not substitutive
- Estimated **~20K incremental DAU** from Android-only GA
- Plan to bring to iOS and web in 2025

## Nuance
The no-cannibalization finding is the most important result beyond the headline metric. It directly answers the question of whether Quick Replies [077], Emoji Reactions, and Toolbar improvements [078] compound or substitute. **They compound.** Users who would have replied via toolbar still do; emoji reactions capture incremental responses from users who wouldn't have replied at all.

The +1% non-sig sends per DAU lift suggests some users who react also go on to compose — reactions may prime engagement rather than replacing composition. The -0.48% non-sig quality opens decrease is within noise and didn't trigger guardrails.

Non-Yahoo recipients in/out of the experiment bucket see emoji reactions rendered as normal email replies, maintaining cross-platform compatibility.

The ~20K DAU estimate is Android-only. If iOS and web replicate similar lifts, the total could be 40-60K+ incremental DAU, making this one of the larger engagement-to-DAU conversions from the RWS squad.
