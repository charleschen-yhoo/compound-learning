---
id: "045"
title: "Exit Intent Notification Upsell (Oasis)"
date: 2025-08-28
source: "Experiment Sheet — Web Notification Upsells - Exit Intent (Oasis); AIDE-6532"
themes: [notifications, desktop, opt-in, upsells]
confidence: high
goal: "dau/revenue"
---

## Hypothesis
Showing a notification opt-in prompt when users move to close/leave the tab (exit intent) will capture users at a high-intent moment.

## Test Design
- **Platform**: Desktop Web (Oasis)
- **Buckets**: 5%
- **Experiment Window**: Aug 14, 2025 – Aug 28, 2025
- **Decision**: GA (Sep 22)

## Outcome
- **Notification opt-in rate**: +0.35%
- **Notifications opened**: +9.50%
- **% UU opened notifications**: +10.22%
- **PV increase**: +9,828 PVs/day

## Nuance
This confirms the finding from [016] that exit intent is the best opt-in moment (+0.58pp in the earlier test). The 9,828 PVs/day is downstream of the opt-in lift — users who opt in come back via notifications. This is a compounding investment: each new opt-in generates future PVs indefinitely. The exit intent pattern avoids the fatigue problem seen in Inbox Refresh Upsell [059] because it triggers only once per session at departure.
