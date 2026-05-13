---
id: "067"
title: "Add a Mailbox Upsell — Failed"
date: 2026-01-01
source: "YMail User Growth Team Cross-BU Presentation (3.6.2026), p25"
themes: [new-users, onboarding, imap-in, failed-experiment]
confidence: high
goal: "dau/revenue"
---

## Hypothesis
Nudging new users who skipped the "add a mailbox" onboarding step to connect another email account (via TOI card) will increase IMAP-in account connections and improve retention by giving users a populated inbox.

## Test Design
- **Platform**: iOS + Android
- **Surface**: Top-of-Inbox (TOI) card, post new user onboarding
- **Target**: New users who skipped the add-a-mailbox module

## Outcome
| Metric | iOS | Android |
|--------|-----|---------|
| Saw upsell | 3,518 | 4,822 |
| Clicked | 211 (6%) | 725 (15%) |
| Added mailbox | 8 (0.2%) | 13 (0.27%) |

**No stats sig impact on % users with IMAP-in account.**

## Nuance
The funnel drop-off is dramatic: Android had 15% CTR but only 0.27% conversion to actually adding a mailbox. The "add a mailbox" action requires significant effort (authenticating with another email provider, waiting for sync) that a simple TOI nudge can't overcome. Users who skipped this during onboarding (when motivation is highest) are unlikely to do it from an inbox card.

This, combined with the newsletter failure [066], suggests that the new user empty inbox problem can't be solved with post-hoc nudges. The team may need to either (a) make the onboarding step itself more compelling/mandatory, or (b) accept that some users will churn and focus on the users who do activate naturally.
