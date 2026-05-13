---
id: "061"
title: "Rich Web Notifications with Icon (Desktop)"
date: 2025-09-01
source: "Experiment Sheet — Web Notifications - Rich Notifications (Norrin, Oasis); AIDE-6533"
themes: [notifications, desktop, engagement, ux-patterns]
confidence: medium
---

## Hypothesis
Adding sender icons to web push notifications will increase CTR and CTP by making notifications more visually informative.

## Test Design
- **Platform**: Desktop Web (Norrin + Oasis)
- **Buckets**: 5%, all OS, all browsers, US and INTL
- **Experiment Window**: Aug 18, 2025 – Sep 1, 2025
- **Decision**: Iterate (rerun with larger buckets and sessions as primary metric)

## Outcome
- **CTR**: Directional increase, not stats-sig
- **CTP**: Increase with stats-sig

## Nuance
The CTP statsig without CTR statsig is interesting — users who do click through are more engaged, but the icon alone doesn't drive more clicks. The team decided to rerun with larger buckets and time-spent/sessions as primary metric rather than CTR, suggesting the value may be in session quality rather than notification click rate. This aligns with the notification redesign with sender pattern [036] on iOS where sender identity lifted engagement.
