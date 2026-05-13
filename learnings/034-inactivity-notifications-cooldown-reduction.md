---
id: "034"
title: "Inactivity Notifications Cooldown Reduction 7→5 Days (Android)"
date: 2024-10-01
source: "Experiment Sheet — Inactivity Notifications: Cooldown from 7 to 5 days (Android)"
themes: [notifications, mobile, engagement, reactivation]
confidence: high
---

## Hypothesis
Reducing the inactivity notification cooldown from 7 days to 5 days will bring users back more frequently without causing notification fatigue.

## Test Design
- **Platform**: Android
- **Project Type**: Engagement-Notif
- **Decision**: GA

## Outcome
**+119,000 DAU** — significant lift from a parameter-level change.

## Nuance
This is a "tuning" experiment — no UX change, just a cadence change. The large impact suggests the 7-day cooldown was overly conservative and many users were ready to re-engage earlier. However, it's important to note that shortening cooldown further (5→3 days) wasn't tested — there's likely a point of diminishing returns where fatigue sets in. Compare to Inbox Refresh Upsell [059] where too-frequent prompts led to complaints and termination.
