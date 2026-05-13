---
id: "062"
title: "Web Notification Action Buttons (Desktop)"
date: 2025-09-03
source: "Experiment Sheet — Web Notifications - Action Buttons (Norrin, Oasis); AIDE-6534"
themes: [notifications, desktop, engagement, ux-patterns]
confidence: medium
---

## Hypothesis
Adding (or removing) action buttons on web push notifications will affect engagement.

## Test Design
- **Platform**: Desktop Web (Norrin + Oasis)
- **Buckets**: 5%, Chrome and Edge only (action buttons are browser-dependent), US and INTL
- **Experiment Window**: Aug 20, 2025 – Sep 3, 2025
- **Decision**: Iterate (rerun with larger buckets and sessions as primary metric)

## Outcome
- **CTR**: Directional increase, not stats-sig
- **CTP**: Increase with stats-sig

## Nuance
Results mirror Rich Notifications [061] exactly — directional CTR, statsig CTP. The browser restriction (Chrome/Edge only) limits the addressable population, which may explain the lack of stats sig on CTR. Compare to mobile Actions on Notifications [039] which showed +47,500 DAU — the concept clearly works on mobile, and the desktop web version needs larger buckets to validate. The team plans to rerun both this and Rich Notifications with sessions/time-spent as primary metric.
