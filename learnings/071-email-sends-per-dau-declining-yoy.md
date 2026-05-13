---
id: "071"
title: "Email Sends Per DAU Declining YoY Across All Platforms"
date: 2024-11-20
source: "Read Write Search Squad MPU Decks, Sept-Nov 2024; Emails Send per DAU Investigation (Keria Bermúdez-Hernández, Oct 28 2024)"
themes: [engagement-features, writing, strategic-context, macro-trend]
confidence: high
goal: "engagement"
---

## Hypothesis
N/A — this is a health metrics investigation into the observed decline in email sends per DAU.

## Test Design
YoY analysis of sends per DAU across platforms using last-28-day rolling averages. Deep-dive investigation by FLAOT segment and region.

## Outcome
**Sends per DAU (September 2024 vs. YoY):**
| Platform | Sends/DAU | MoM | YoY |
|----------|-----------|-----|-----|
| Android | 0.21 | +8.6% | -2.9% |
| iOS | 0.16 | +16.9% | -8.9% |
| Desktop | 0.55 | +6.0% | -14.6% |

**By November 2024**, mobile send per DAU dropped further to 0.17 (78% of 0.22 goal). Desktop flat at 0.58 (79% of 0.73 goal). iOS -2% MoM, Android -3% MoM.

**FLAOT Segment Breakdown (Sept 2024 YoY):**
| Segment | iOS YoY | Android YoY |
|---------|---------|-------------|
| Fanatic | -9.16% | -1.90% |
| Loyalist | -4.87% | -5.46% |
| Active | +0.85% | -5.46% |
| Occasional | -14.76% | -10.24% |
| Tourist | varies | -2.23% |

Occasional users are hit hardest on both platforms. The decline is visible across all FLAOT segments, both US and INTL.

**Regional Breakdown:**
- iOS: US -9.3%, INTL -8.9%
- Android: US -2.7%, INTL -3.4%

**Root causes identified:**
- **iOS**: SDK fix in Sept inflated MoM; YoY driven by lower share of very engaged users + general trend
- **Android**: General trend of users sending fewer emails
- **Desktop**: Primarily an instrumentation change in April that lowered the 2024 baseline by -7% to -12%. Pre-instrumentation change snapshot (March 2023 to 2024) still showed -7%, confirming an underlying decline

**Cannot determine if macro or O&O-specific** — no IMAP-Out send data available.

**Team's next steps (as of Oct 2024):**
1. Prove whether sends/IMAP-Out DAUs is also declining — seek proxy data
2. If O&O-only: look at compose in-flow sources (reply/forward/new) to find which are leaking; prioritize fixing high-volume flows in Q1 2025
3. If macro: confirm with industry data; explore new ways to send (universal messenger, emoji reactions) to correct the downtrend

## Nuance
The team explicitly noted in November 2024 that "we haven't fully realized Android GA gains from Quick Replies — however those gains may not overtake send pattern loss." This is a critical admission: **feature-level engagement wins may be insufficient to offset the macro decline.**

Write is the weakest of the three RWS metrics: 78-79% of goal vs Read at 84-90% and Search at 93-101%. Mobile search actually **hit 101% of goal** (62.62% vs 62% target) by November — making the sends decline stand out even more starkly.

Desktop's disproportionate decline (-14.6% YoY) aligns with the broader pattern of desktop engagement declining faster than mobile [026], but the instrumentation change accounts for roughly half of it.

The FLAOT breakdown showing Occasional users declining fastest (-14.76% iOS, -10.24% Android) is strategically significant: these are the users gamification targets [006, 008]. If Occasional users are sending fewer emails, the gamification thesis may need to expand beyond "come back more often" to "do more while you're here."
