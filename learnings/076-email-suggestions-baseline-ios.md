---
id: "076"
title: "Email Suggestions Baseline iOS — Removal Caused -2.76% Search Success"
date: 2024-11-01
source: "Read Write Search Squad MPU Decks, Sept-Nov 2024"
themes: [engagement-features, search, mobile, suggestions]
confidence: high
goal: "engagement"
---

## Hypothesis
By disabling email suggestions for mobile app Mail search users, we expect to see a neutral impact on our average search success metric because we are just trying to better understand how email suggestions impact our overall average search success rate.

## Test Design
- **Platform**: iOS
- **Type**: Holdback/removal test — removed email suggestions to measure their baseline impact
- **Metric**: Search success rate, suggestion CTR

## Outcome
- **Approx -2.76% decline in search success rate** when suggestions were removed
- Control (with suggestions) had higher CTR in the non-empty state: **14% vs 10.5%** for the test variant
- Decision: **keep suggestions on iOS, expand to Android**

**Detailed CTR by suggestion type (control / non-empty state):**
| Type | Shown Count | Selected | CTR |
|------|-------------|----------|-----|
| Contacts | 7,042,975 | 1,298,665 | 18.44% |
| Email Suggestions | 3,849,091 | 361,005 | 9.38% |
| Suggested Keywords | 1,196,298 | 106,220 | 8.88% |
| Recent | 1,562,588 | 179,607 | 11.49% |

Contacts had the highest CTR (18.44%), followed by Recent (11.49%), Email Suggestions (9.38%), and Keywords (8.88%).

## Nuance
The hypothesis was intentionally conservative ("expect neutral") — the team designed this as a baseline measurement, not an optimization experiment. The -2.76% result exceeded expectations, confirming suggestions are a meaningful contributor to search quality.

The CTR hierarchy — Contacts > Recent > Email Suggestions > Keywords — reveals what users value most in pre-search: **who sent it** (contacts) and **what they recently searched** (recents). This aligns with the finding that transaction email lookup is the top search use case [075].

The recommendation to expand to Android is the direct next step: Email Suggestions Android is planned for 7.55. If Android shows a similar ~2.76% lift from adding suggestions (vs the iOS lift from *not* removing them), this becomes one of the highest-leverage search improvements available.

This baseline validation approach (remove to measure) is a useful methodology when a feature has been live long enough that its incremental value is unknown.
