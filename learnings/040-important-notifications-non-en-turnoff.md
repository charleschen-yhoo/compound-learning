---
id: "040"
title: "Important Notifications: Turn Off for Non-EN Users (Android)"
date: 2024-10-01
source: "Experiment Sheet — Important Notifications: Turn off for non-EN Users (Android)"
themes: [notifications, mobile, internationalization, engagement]
confidence: high
---

## Hypothesis
The "important email" classification model is less accurate for non-English languages, so turning off important notifications for non-EN users (and reverting to all-email notifications) may actually improve engagement by reducing false negatives.

## Test Design
- **Platform**: Android
- **Project Type**: Engagement-Notif
- **Decision**: GA

## Outcome
**+29,000 DAU** — turning off the filtering for non-EN users was a net positive.

## Nuance
This is a counterintuitive result: *removing* a feature (important email filtering) improved metrics for a specific segment. It suggests the importance classifier's accuracy varies by language, and for non-EN users, the false negative rate (missing actually-important emails) was worse than the noise of sending all notifications. This is an important data point for INTL expansion of any ML-based feature — the English-trained model doesn't automatically transfer.
