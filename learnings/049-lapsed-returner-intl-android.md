---
id: "049"
title: "Lapsed Returner Notification Upsell INTL (Android)"
date: 2025-10-28
source: "Experiment Sheet — Lapsed Returner Notification Upsell INTL (Android); AIDE-6828"
themes: [notifications, mobile, internationalization, reactivation]
confidence: high
---

## Hypothesis
The lapsed returner notification upsell, which worked domestically [047], will also work for international (non en-US) Android users.

## Test Design
- **Platform**: Android (v7.74.1)
- **Buckets**: 5%, non en-US users only
- **Experiment Window**: Oct 14, 2025 – Oct 28, 2025
- **Decision**: GA
- **Note**: iOS INTL version needed re-run

## Outcome
- **DAU**: +4,738
- **ARPU**: +$63/day

## Nuance
This is one of the few experiments that quantifies both DAU and revenue impact. The +$63/day ARPU validates that INTL notification upsells drive not just engagement but monetizable engagement. The iOS INTL version iterated (needs re-run), consistent with the pattern that Android notification experiments tend to GA more readily than iOS. The domestic Android version [047] yielded +4,592 DAU — nearly identical, suggesting INTL users respond at similar rates.
