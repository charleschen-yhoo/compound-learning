---
id: "059"
title: "Inbox Refresh Notification Upsell — Terminated"
date: 2025-10-01
source: "Experiment Sheet — Web Notifications Upsells - Inbox Refresh Upsell (Oasis); AIDE-6686"
themes: [notifications, desktop, opt-in, upsells, failed-experiment]
confidence: high
goal: "dau/revenue"
---

## Hypothesis
Prompting users to enable notifications each time they refresh their inbox will increase the opted-in base.

## Test Design
- **Platform**: Desktop Web (Oasis)
- **Buckets**: 10%, same layer as cooldown timer upsells
- **Experiment Window**: Sep 17, 2025 – Oct 1, 2025
- **Decision**: Terminated

## Outcome
**Decrease in DV. User complaints about too many upsells.**

## Nuance
This is the clearest negative signal in the notification upsell portfolio. While exit intent [045] and message read [050] upsells work because they're contextually appropriate (leaving / just engaged with content), the inbox refresh moment is too frequent and feels intrusive. Users refresh their inbox many times per session — hitting them with an upsell each time crosses the line from "helpful reminder" to "nagging." This establishes a boundary: notification upsells should be triggered by meaningful user actions (reading, leaving), not by ambient/frequent actions (refreshing). The DV decrease suggests it didn't just fail to help — it actively hurt engagement.
