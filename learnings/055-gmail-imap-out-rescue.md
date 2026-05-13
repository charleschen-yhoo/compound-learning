---
id: "055"
title: "Gmail IMAP-Out Rescue (iOS + Android)"
date: 2025-01-05
source: "Experiment Sheet — Gmail IMAP-Out Rescue (Identity, Android + iOS)"
themes: [imap-out-rescue, acquisition, gmail]
confidence: high
goal: "dau/revenue"
---

## Hypothesis
The IMAP-Out Rescue flow that works for Apple Mail users can be adapted for Gmail users who have Yahoo accounts connected via IMAP to Gmail.

## Test Design
- **Platform**: Identity (Android + iOS)
- **Project Type**: Acquisition
- **Experiment Window**: Nov 21-22, 2024 – Jan 5, 2025
- **Decision**: GA on both platforms

## Outcome
- **Android**: 1,243 downloads/day
- **iOS**: 537 downloads/day
- **Combined**: ~1,780 downloads/day

## Nuance
Gmail IMAP-Out Rescue yields far lower volume than Apple Mail Rescue (1,780/day vs 55,700 DAU [038]). This likely reflects two factors: (1) fewer Yahoo users connect via Gmail IMAP than Apple Mail IMAP, and (2) Gmail users may be more committed to their existing client. Still, the downloads are incremental and the marginal cost of adding Gmail as a rescue surface is low since the infrastructure already exists. The Android/iOS split (70/30) mirrors the overall IMAP-Out pattern. This extends the rescue surface taxonomy beyond Apple Mail, Samsung Mail (terminated — Samsung blocks deep links), and desktop.
