---
id: 082
title: "Registration-events join lags ~6 weeks; first-active SID cohorts count identity churn as new users"
date: 2026-08-19
source: "DS review + cohort_retention_daily_segmented cross-checks + 2025 backtest"
themes: [measurement, retention, data-quality]
confidence: high
goal: "dau/revenue"
---

## Hypothesis

Registration cohorts joined to events (user_id = sob) and the DE first-active retention table should tell the same retention story.

## Test Design

Same cohorts computed through both pipelines; 2025 history pulled from the DE table as a backtest; April 2026 anomaly investigated against registration volumes.

## Outcome

Two independent failure modes. (1) The user_id = sob join does not reliably match for several weeks after account creation: August cohorts read ~5pp low on the join-based method while April cohorts matched within 0.5pp. Any join-based read on cohorts younger than ~6 weeks understates retention. (2) The DE table cohorts on first-seen SID, so cookie resets and forced logouts mint fake "new users": its cohort sizes run 15-40% above actual registrations, early-2025 desktop cohorts ran ~4x registrations during peak IMAP-out logout waves, and April 2026 showed a cross-platform cohort spike while actual signups were at their yearly trough.

## Nuance

Neither source is wrong, they answer different questions. Join-based = "do accounts we created come back" (trustworthy only for matured cohorts). First-active = "do newly seen identities come back" (fresh and join-free, but identity churn contaminates it). For MPU we present raw registration cohorts Jan-Jul only, and treat both alternatives as labeled cross-checks.
