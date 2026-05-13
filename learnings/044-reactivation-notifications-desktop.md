---
id: "044"
title: "Web Reactivation Notifications (Desktop)"
date: 2025-09-12
source: "Experiment Sheet — Web Notifications - Reactivation Notifications (Norrin, Oasis); AIDE-6567"
themes: [notifications, desktop, reactivation, engagement]
confidence: high
goal: "dau/revenue"
---

## Hypothesis
Sending web push notifications to logged-out or inactive desktop users will bring them back to Yahoo Mail.

## Test Design
- **Platform**: Desktop Web (Norrin + Oasis)
- **Buckets**: 5%
- **Targeting**: Windows only, all browsers, US and INTL users
- **Experiment Window**: Aug 18, 2025 – Sep 12, 2025
- **Decision**: GA

## Outcome
- **+10,435 PVs/day** once GA'd
- **Notification opened**: +1.20%
- **Logged-out notification CTP**: +4.00%

## Nuance
This is a uniquely powerful capability — web push notifications can reach users even when they're logged out, which mobile push cannot. The +4% CTP on logged-out users represents a re-engagement channel that doesn't exist on mobile. This validates the opportunity identified in [016] about using notifications for logged-out user re-engagement. Expanding to MacOS (currently Windows-only) should roughly double impact per [001] pattern.
