---
id: "053"
title: "Move Push Notification Onboarding to Position 1 (iOS)"
date: 2024-08-14
source: "Experiment Sheet — Move Push Notification Onboarding to Position 1 Redo - bcookie (iOS)"
themes: [notifications, mobile, onboarding, opt-in]
confidence: high
goal: "dau/revenue"
---

## Hypothesis
Moving the push notification permission prompt to the first position in the onboarding flow (before other setup steps) will increase opt-in rates.

## Test Design
- **Platform**: iOS
- **Project Type**: Engagement-Notif
- **Experiment Window**: Jul 8, 2024 – Aug 14, 2024
- **Decision**: GA
- **Note**: Android version was terminated

## Outcome
**+2,400 DAU** — positioning the notification ask first in onboarding works on iOS.

## Nuance
The iOS success vs Android termination parallels the broader pattern: iOS notification experiments have different dynamics than Android. The "bcookie" redo tag suggests this was a rerun addressing tracking issues. While 2,400 DAU is modest, the opt-in is permanent and compounds — every new user who opts in during onboarding generates future engagement. This is an upstream lever: growing the opted-in base makes all downstream notification experiments (sticky [001], reactivation [044], actions [039]) more impactful.
