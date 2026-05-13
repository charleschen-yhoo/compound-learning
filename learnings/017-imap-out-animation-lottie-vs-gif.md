---
id: 017
title: "IMAP-Out Rescue Animation Optimization (Lottie vs GIF)"
date: 2025-04-24
source: "UG Squad MPU - April 2025"
themes: [imap-out-rescue, performance, acquisition, international]
confidence: high
goal: "dau/revenue"
---

## Hypothesis

Replacing GIF animations with Lottie in the IMAP-Out Rescue flow will reduce file size, improve performance, and lift downloads — particularly on Android and in emerging markets with higher device variability.

## Test Design

Default (GIF) vs Challenger (Lottie) on both Android and iOS IMAP-Out Rescue upsell screens. No UI changes — only the animation format.

## Outcome

74% average file size reduction. Android: +5.7% lift in downloads, +8% button CTR. iOS: +1.4% downloads, +1.8% button CTR. 131K incremental downloads projected by EOY → 37.5K DAU. Country breakdown: Egypt +13.25%, Nigeria +12.51%, Philippines +10.62%, Indonesia +7.96%, India +6.55%, US +3.99%.

## Nuance

Confirmed the hypothesis that impact correlates with device variability and performance constraints. Emerging markets with Android-heavy, lower-spec device populations saw double-digit lifts. The US saw a more modest +3.99%. This validates that performance optimization is a growth lever, especially for international expansion — not just a tech-debt initiative.
