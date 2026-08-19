---
id: 081
title: "Gating retention on a window that contains the measured day is circular"
date: 2026-08-19
source: "DS review of the New Accounts workbook (Atlanta Gao) + fixed-query rerun"
themes: [measurement, retention, new-users]
confidence: high
goal: "dau/revenue"
---

## Hypothesis

Gating D1/D7 retention on "activated" users (any active event in days 0-7) should give a cleaner read of real-user retention than raw registration cohorts.

## Test Design

Algebraic review plus a live rerun of the corrected query against BigQuery, cross-checked against the join-free DE retention table.

## Outcome

The gate was a tautology for D1 and D7: anyone active on day 1 or day 7 is automatically inside the day 0-7 activation window, so the gate never filtered the numerator. Gated rate = raw rate / activation rate, always. Proven with the January Desktop Web x US cohort: identical numerator (130,709), only the denominator shrank (24.2% -> 28.3% = 24.2 / 85.4%). The fix is to gate on day 0 only, which is disjoint from every measured day; with that fix, April's number landed within 0.5pp of the independent join-free source.

## Nuance

D28 was never affected (day 28 falls outside the activation window). The circular version was not just uninformative, it was actively worse: any move in the activation rate (like the 5/1 active_uu_flag widening) moved gated D1 mechanically with zero behavior change. General rule: the qualifying condition and the measured outcome must be disjoint in time.
