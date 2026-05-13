---
id: "050"
title: "Message Read Notification Upsell Rerun (Oasis)"
date: 2025-09-12
source: "Experiment Sheet — Web Notification Upsells - notifReadUpsell re-run (Oasis); AIDE-6568"
themes: [notifications, desktop, opt-in, upsells]
confidence: high
goal: "dau/revenue"
---

## Hypothesis
Prompting users to enable notifications immediately after they read an email creates a contextually relevant opt-in moment.

## Test Design
- **Platform**: Desktop Web (Oasis)
- **Buckets**: 10%, same layer as Exit Intent Upsell
- **Experiment Window**: Aug 28, 2025 – Sep 12, 2025
- **Decision**: GA

## Outcome
For eligible users:
- **Notification opt-in rate**: +0.74%
- **Notifications opened**: +57.26%
- **% UU opened notifications**: +0.22%
- **PV increase**: +1.72% (0.42% overall)

## Nuance
The +57.26% increase in notifications opened is striking — users who opt in at the message-read moment are highly engaged with notifications afterward. The 0.74% opt-in rate is higher than exit intent's 0.35% [045], suggesting the message-read moment is even more contextually relevant. However, the overall PV lift (0.42%) is lower than exit intent's 9,828 PVs/day, possibly because message-read eligible users are already more engaged (they're actively reading email). The two upsells are complementary and run on the same layer.
