# IMAP-Out Rescue & Acquisition

## Summary

IMAP-Out Rescue is the team's primary growth engine, driving app downloads by intercepting users who access Yahoo Mail via third-party email clients (Apple Mail, Gmail, etc.) and encouraging them to download the Yahoo Mail app. The program has scaled from ~5K daily downloads in early 2025 to 24K+ by mid-2025 through a compounding series of creative, UX, and performance optimizations. Logout campaigns are the second major pillar, generating 1.1M+ DAU in 2026 by forcing IMAP-Out users to re-authenticate through Yahoo's own surfaces.

## Confidence-Ranked Findings

**High Confidence:**
- IMAP-Out-Only logout yields 6% DAU with no degradation over time — a proven compounder [012]
- Creative optimizations compound: Lottie (+5.7% Android) + spam-fighting animation (+22%) + "Maybe Later" removal (+16%) together scaled downloads from 5K to 24K/day [017, 018, 020]
- Removing false choices ("Maybe Later") increases conversion when users are high-intent [018]
- Performance optimization (Lottie) has outsized impact in emerging markets with device variability (Egypt +13.25%, Nigeria +12.51%) [017]

**Medium Confidence:**
- O&O + IMAP-Out segment yields 2.5% steady-state — less than half of IMAP-Out-Only — because these users have alternative first-party access [013]
- New IMAP-Out surfaces (password screen toast) have very low CTR (0.05%) but high install rate (33.3%) among clickers — incremental but small [002]
- D30 retention (17% Android, 11% iOS) is the next bottleneck — a 1-2% improvement = +35K DAU [027]

## Contradictions
- **Removing friction helped in IMAP-Out** (removing "Maybe Later": +16% downloads) but **didn't help in engagement features** (auto subject line: no DV impact, infinite scroll: no topline impact). See main synthesis for hypothesis.

## Open Questions
- What is the steady-state yield for 2nd logouts (re-logouts of the 40M+ pool)?
- Why is iOS retention (11%) lower than Android (17%) for IMAP-Out Rescue users?
- Can IMAP-Out Rescue expand to desktop email clients?

## Opportunity Areas
- **Retention optimization**: Downloads are solved; retention is the next frontier. Onboarding experiments are the active lever.
- **International expansion**: Lottie results show emerging markets respond strongly to performance improvements. Targeted optimization for high-volume, low-spec markets.
- **Device launch planning**: iPhone 17 drove 105K downloads in 7 days [028]. Preparing optimized experiences around predictable device launches.

## Related Learnings
[002, 012, 013, 017, 018, 019, 020, 027, 028, 029]
