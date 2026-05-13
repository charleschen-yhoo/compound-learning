---
id: "039"
title: "Actions on Notifications (iOS + Android)"
date: 2024-10-01
source: "Experiment Sheet — Actions on Notifications (Android), Actions on Notification Long Press (iOS)"
themes: [notifications, mobile, engagement, ux-patterns]
confidence: high
goal: "dau/revenue"
---

## Hypothesis
Adding actionable buttons (mark read, delete, reply) directly on push notifications will increase engagement by letting users triage without opening the app.

## Test Design
- **Platform**: iOS (long press) + Android (direct actions)
- **Project Type**: Engagement-Notif
- **Decision**: GA on both platforms

## Outcome
- **Android**: +32,500 DAU
- **iOS** (long press): +15,000 DAU
- **Combined**: +47,500 DAU

## Nuance
Android's higher impact likely reflects the platform's more prominent notification action affordance vs iOS requiring long press. This validates the core loop insight [030] — the primary email actions are open/delete/click, and enabling those actions directly from notifications reduces the friction to triage. The Android vs iOS gap (~2x) may inform prioritization for future notification features.
