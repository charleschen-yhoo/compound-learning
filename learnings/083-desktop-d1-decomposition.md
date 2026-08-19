---
id: 083
title: "Desktop web D1 decline decomposed: one third tagging bug, two thirds traffic mix; product stable"
date: 2026-08-19
source: "New Accounts workbook D1 walk + property-level queries (Jan vs Jul 2026)"
themes: [retention, new-users, instrumentation, acquisition-quality]
confidence: high
goal: "dau/revenue"
---

## Hypothesis

Desktop web D1 fell from 24.2% (Jan) to 20.1% (Jul); is the product retaining worse?

## Test Design

Mix/rate decomposition by signup flow, then by source property (reg_source_spaceid), with pre/post falsification tests around suspected change dates and an engagement-gated cross-check.

## Outcome

No product problem. The -4.1pts splits: (1) -1.4pts from a 7/15 deploy that stopped stamping platform/country on mail-direct registrations (verified: volume conserved day-by-day, de-stamped users retain at 27.7% like mail-direct, Unknown bucket stepped up +1.3pts the same day); (2) -0.6pts from a Yahoo Finance sign-in prompt minting accounts via one-click Google SSO at 9x volume - their Mail D1 was ALWAYS ~4.5%, only volume changed; (3) -2.1pts of traffic-quality drift on the login page and signup landing pages (pages steady, visitors changed), correlated with the performance marketing push that flows through by August. Users who engage on day one retain unchanged throughout.

## Nuance

The headline lesson is procedural: decompose before narrating. Three successive framings ("web is leaking", "mostly measurement", "one broken flow") were each partly wrong until the property-level cut. Also: a flow-level "quality collapse" (ybar 14.9% -> 4.8%) can be pure mix - no property's rate moved. Fall checkpoint: if the marketing correlation is right, login/signup-page D1 recovers in Sep-Oct cohorts.
