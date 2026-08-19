---
id: 084
title: "Signup type drives retention: iOS native beats Google SSO 11.5 vs 7.9 D28; Android reverses"
date: 2026-08-19
source: "sigtype_retention.sql, May-Jun 2026 US cohorts, raw exact-day basis"
themes: [retention, new-users, onboarding, siwg]
confidence: medium
goal: "dau/revenue"
---

## Hypothesis

Team POP baselines suggested Gmail-connected signups retain worse than native on iOS but slightly better on Android; verify on our own basis.

## Test Design

May-June US registration cohorts split by reg_category (tpa-google = Google SSO vs native flows), exact-day D1/D7/D28.

## Outcome

Both directions confirmed. iOS: native (uid) D28 11.5% vs Google SSO 7.9%. Android: Google SSO 8.9% vs native blend ~7.2%. Two surprises: Android has two native flows with a 10pt D1 gap (uid 32.2% vs username 22.0% - what separates them is unknown and potentially a lever), and iOS carries a junk-like username bucket (41K signups at D1 2.8%) diluting its averages.

## Nuance

reg_category semantics differ by platform and are undocumented - definitions need Identity confirmation before building on this. Confidence medium until the uid/username split is understood. The iOS native-vs-SSO gap is the quantified prize for the SIWG onboarding revamp.
