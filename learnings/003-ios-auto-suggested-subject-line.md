---
id: 003
title: "iOS Auto Suggested Subject Line"
date: 2026-04-23
source: "UG Squad MPU - April 2026"
themes: [ai-features, compose, engagement]
confidence: high
goal: "dau/revenue"
---

## Hypothesis

Using on-device LLM to auto-suggest subject lines when users attempt to send without one will reduce compose friction and drive higher sends/sender and DV.

## Test Design

iOS users eligible if: attempting to send without a subject, iOS 26+, iPhone 15 Pro+, en-US, Apple Intelligence enabled. Control: no subject prompt. Treatment: system-generated subject line suggestion. Measured sends w/o subject rate, sends/sender with subject, total sends/sender, suggestion acceptance rate.

## Outcome

% sends without subject dropped from 89% (control) to 69% (treatment) — 3x more emails sent with subjects. Sends/sender with subject: 0.21 (control) vs 0.58 (treatment). Total sends/sender: 2.30 vs 2.30 (flat). Suggestion acceptance: 18%. No impact on overall send volume or engagement.

## Nuance

The feature works — users adopt it — but it doesn't drive incremental engagement. Users who found subjects hard to compose showed clear trust in the feature, increasingly sending without knowing AI would catch them. The hypothesis that lowering compose friction would drive higher sends/sender and DV didn't play out. However, the results point to a clear path for leveraging AI to make writing emails easier, even if the topline engagement impact is neutral.
