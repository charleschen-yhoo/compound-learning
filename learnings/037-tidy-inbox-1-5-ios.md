---
id: "037"
title: "Tidy Inbox 1.5 (iOS)"
date: 2024-11-13
source: "Experiment Sheet — Tidy Inbox 1.5 (iOS)"
themes: [engagement, triage, mobile, tidy-inbox]
confidence: high
---

## Hypothesis
Tidy Inbox (automated inbox cleanup suggestions) will drive engagement by helping users manage email overload.

## Test Design
- **Platform**: iOS
- **Project Type**: Engagement-Feature
- **Experiment Window**: Sep 30, 2024 – Nov 13, 2024
- **Decision**: GA (ramped existing bucket to 100%)
- **Note**: Android version ran in parallel but was iterated — strong engagement only at highest FLAOT level, needed broadening

## Outcome
**+96,510 DAU** on iOS — GA'd. Android iterated due to engagement concentrated in Fanatic segment only.

## Nuance
The iOS/Android split is revealing: the same feature worked broadly on iOS but only for power users on Android. This could reflect differences in how iOS vs Android users manage email, or platform-specific UX differences in how Tidy Inbox was surfaced. The Android limitation (engagement only at highest FLAOT) is the opposite of the gamification pattern [006, 008] where Occasional/Tourist users responded most strongly. Tidy Inbox may appeal to users who already care about inbox hygiene (Fanatics) rather than creating new behavior.
