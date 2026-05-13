---
id: "069"
title: "Onboarding Is Structurally Constrained"
date: 2026-03-06
source: "YMail User Growth Team Cross-BU Presentation (3.6.2026), p19-20"
themes: [new-users, onboarding, strategic-context, failed-experiment]
confidence: high
goal: "dau/revenue"
---

## Hypothesis
N/A — this is a strategic assessment of why onboarding experiments consistently fail.

## Test Design
N/A — analysis of constraints across impact, infrastructure, and data.

## Outcome
Three categories of constraints prevent effective onboarding optimization:

**Impact constrained:**
- New accounts < 1% of DAU (57K/day)
- D7 retention: 12%, D90 retention: 7%
- Even doubling D90 = only 200K incremental DAU (meaningful but small relative to notification/IMAP-Out levers)

**Infrastructure constrained:**
- Evaluate buckets can't reliably support onboarding experiments
- The full onboarding journey spans 3 properties (marketing website, signup flow, mail app) — data doesn't carry across
- IMAP-In mailboxes take time to download, making the first session experience poor

**Data constrained:**
- Don't know where users come from (source not maintained)
- Don't know user's JTBD or what features they value
- Users come into an empty inbox

## Nuance
This is the "why" behind multiple failed onboarding experiments: newsletter recommendations [066], add a mailbox upsell [067], and others referenced in the deck ("even when we tried, experiments fell flat"). The constraints are structural, not tactical — it's not that the team picked the wrong experiments; it's that the experimentation surface itself is hostile.

The 35%+ registration traffic from "unknown" source (identified as IMAP) means the team doesn't even know who a large portion of new users are. Combined with the empty inbox problem, new users face: unknown source → empty inbox → no JTBD signal → generic experience → 88% churn by D7.

The strategic implication: given the constraints, the team has rationally deprioritized onboarding in favor of higher-leverage areas (notifications, IMAP-Out Rescue, gamification). This is a correct prioritization given the math — 267K DAU from web notifications [031] vs 200K DAU from doubling onboarding retention.
