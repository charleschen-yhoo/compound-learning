---
id: "060"
title: "Sticky Summary Notifications (Desktop)"
date: 2025-09-29
source: "Experiment Sheet — Web Notifications - Sticky Summary Notifications (Norrin, Oasis); AIDE-6685"
themes: [notifications, desktop, engagement]
confidence: medium
---

## Hypothesis
Making summary notifications (inbox digest) sticky (persistent until dismissed) will increase notification engagement.

## Test Design
- **Platform**: Desktop Web (Norrin + Oasis)
- **Buckets**: 10%, all OS, all browsers, US and INTL
- **Experiment Window**: Sep 15, 2025 – Sep 29, 2025
- **Decision**: On hold (bug in service worker)

## Outcome
**Positive CTR and CTP gains**, but no stats-sig PV lift — potentially due to service worker bug.

## Nuance
Like Sticky Important Notifications [001], making notifications persistent increases engagement with the notification itself. However, the PV lift didn't materialize, possibly because summary notifications are less urgent than "important email" notifications — users see the summary but don't feel compelled to click through. The service worker bug adds uncertainty; a clean rerun is needed. If the bug was causing notification delivery failures, the true impact could be substantially higher. This is the second experiment (along with [001]) impacted by the same service worker bug.
