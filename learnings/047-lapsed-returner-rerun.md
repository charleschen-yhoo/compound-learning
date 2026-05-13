---
id: "047"
title: "Lapsed Returner Notification Upsell Rerun (iOS + Android)"
date: 2025-05-15
source: "Experiment Sheet — Lapsed Returner Notification Upsell Rerun (iOS, Android)"
themes: [notifications, mobile, reactivation, opt-in]
confidence: high
---

## Hypothesis
Users who have returned after a lapse are in a high-intent moment and more receptive to enabling push notifications.

## Test Design
- **Platform**: iOS (v7.63) + Android (v7.64)
- **Project Type**: Engagement-Notif
- **First runs**: Had bugs in trigger logic, needed re-launch
- **Decision**: GA on both

## Outcome
- **iOS**: +1,648 DAU
- **Android**: +4,592 DAU
- **Combined**: +6,240 DAU

## Nuance
The "lapsed returner" targeting is smart — these users have already demonstrated re-engagement intent by coming back, making the notification ask feel natural rather than pushy. Android outperforms iOS ~3:1, consistent with the pattern seen in nudges [046] and actions on notifications [039] where Android's notification system is more permissive. The INTL extension [049] adds another +4,738 DAU on Android alone, suggesting significant headroom in non-EN markets.
