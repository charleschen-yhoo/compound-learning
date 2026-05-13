---
id: "048"
title: "Persistent Reminder to Turn on Notifications (iOS + Android)"
date: 2025-06-05
source: "Experiment Sheet — Persistent Reminder to Turn on Notifications (iOS Rerun, Android)"
themes: [notifications, mobile, opt-in, engagement]
confidence: high
---

## Hypothesis
A persistent (recurring) reminder to enable push notifications will grow the opted-in base by catching users at different moments.

## Test Design
- **Platform**: iOS (v7.65, rerun after instrumentation issues) + Android (v7.62)
- **Project Type**: Engagement-Notif
- **Decision**: GA on both

## Outcome
- **iOS** (rerun): +2,884 DAU
- **Android**: +2,258 DAU
- **Combined**: +5,142 DAU

## Nuance
The persistent approach is lower-impact than nudges [046] (+9,122 DAU) but complementary — different users respond to different prompt styles. The first iOS run had instrumentation issues, requiring a rerun. The INTL expansion [042] of this same pattern yielded +20K DAU on iOS alone, suggesting the domestic market may be more saturated for this approach while INTL has more headroom. The Android INTL version had a bug that muddied results.
