---
id: "046"
title: "Nudges for Notification Opt-In v2 Rerun (Android)"
date: 2025-04-01
source: "Experiment Sheet — Nudges for Notification Opt-In v2 Rerun (Android)"
themes: [notifications, mobile, opt-in, nudges]
confidence: high
goal: "dau/revenue"
---

## Hypothesis
In-app nudges prompting users to enable push notifications can grow the notification-opted-in base on Android.

## Test Design
- **Platform**: Android (v7.60)
- **Project Type**: Engagement-Notif
- **Experiment Window**: Mar 10, 2025 – Apr 1, 2025
- **Decision**: GA
- **Note**: v1 was terminated (issues), v2 first run iterated, this is the v2 rerun

## Outcome
**+9,122 DAU** — after two iterations, the nudge pattern works on Android.

## Nuance
It took three attempts to get this right (v1 terminated, v2 iterated, v2 rerun GA'd). The iOS v2 rerun was also iterated (not GA'd), suggesting the nudge pattern is harder to land on iOS where Apple's notification permission system is more rigid. The lesson: notification opt-in nudges are valuable but require iteration — the difference between a good and bad nudge is large. Compare to the persistent reminder approach [048] which also works but at lower DAU scale.
