---
id: "033"
title: "Important Email Notifications (Android)"
date: 2024-10-01
source: "Experiment Sheet — Important Email Notifications (Android)"
themes: [notifications, mobile, engagement]
confidence: high
---

## Hypothesis
Surfacing only important emails via push notifications (filtering out low-value notifications) will increase notification engagement and drive DAU.

## Test Design
- **Platform**: Android
- **Project Type**: Engagement-Notif
- **Decision**: GA
- **Note**: Team decided not to GA for all users initially — ran follow-up experiment with users on "High-priority messages only" setting

## Outcome
**+166,000 DAU** — third-largest engagement experiment in the corpus.

## Nuance
The team iterated on this for non-EN users separately [040]. The initial GA was for EN users, with a subsequent decision to turn off for non-EN users where the relevance model was less accurate. This suggests notification quality (important vs. all) matters more than notification volume — a theme that appears across sticky notifications [001] and notification redesign [036].
