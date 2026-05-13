---
id: "066"
title: "Newsletter Subscription Recommendations — Failed"
date: 2026-01-10
source: "YMail User Growth Team Cross-BU Presentation (3.6.2026), p21-23"
themes: [new-users, onboarding, engagement, failed-experiment]
confidence: high
---

## Hypothesis
Recommending popular Yahoo newsletters (Ball Don't Lie, Get to the Points, Engadget Deals, etc.) to new and lowly-engaged users with empty inboxes will give them a reason to return, driving +58K DAU via DV14 impact.

## Test Design
- **Platform**: iOS + Android
- **Surfaces**: New user onboarding flow + existing user start session
- **Prior signal**: A previous Norrin experiment with 3 options beat control by 1% on D7
- **Goal**: Impact DV14

## Outcome
**Only 0.3% of eligible users signed up for newsletters on either platform.** Experiment terminated.

## Nuance
Two distinct failure modes:
1. **Users perceived the upsell as an advertisement for Yahoo properties**, not a helpful content recommendation. This is a framing problem — the same content offered as "stay informed" vs "subscribe to Yahoo newsletters" triggers different user responses.
2. **Eligibility rate among new downloads was extremely low** because the client didn't receive necessary information from API calls quickly enough during onboarding. This is an infrastructure constraint that affects all onboarding experiments.

The broader learning: the empty inbox problem for new users is real (identified on p19 of the deck), but solving it by pushing Yahoo's own content doesn't work. Users who create a new email account want to use it for *their* communications, not consume Yahoo content. A connected mailbox (IMAP-in) would be more valuable than newsletters, but the Add a Mailbox upsell [067] also failed.
