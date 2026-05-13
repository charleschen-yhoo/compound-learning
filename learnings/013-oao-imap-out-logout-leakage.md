---
id: 013
title: "O&O + IMAP-Out Logout Segment Leakage"
date: 2026-01-22
source: "UG Squad MPU - January 2026"
themes: [imap-out, logout, segmentation, retention]
confidence: high
goal: "dau/revenue"
---

## Hypothesis

The O&O + IMAP-Out segment (users who access Yahoo Mail via both first-party and third-party clients) would convert similarly to the IMAP-Out-Only segment when logged out.

## Test Design

Two logout campaigns targeting O&O + IMAP-Out users. Campaign 1: 49K users logged out on 11/6. Campaign 2: 987K users logged out on 12/18.

## Outcome

Both campaigns showed strong early conversion: Campaign 1 peak yield 5.5%, Campaign 2 peak yield 5.1%. However, steady-state yield for both settled at 2.5% — significantly more leakage than IMAP-Out-Only's sustained 6%.

## Nuance

The O&O + IMAP-Out segment behaves fundamentally differently from IMAP-Out-Only. These users already have access to Yahoo Mail through first-party surfaces, so the logout is less disruptive — they have alternatives. The 2.5% steady-state vs 6% for IMAP-Out-Only confirms that segment-level targeting matters enormously. The O&O segment is a 25M pool but yields less than half per user.
