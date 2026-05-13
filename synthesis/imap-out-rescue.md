# IMAP-Out Rescue & Acquisition

## Summary

IMAP-Out Rescue is the team's most developed growth lever, with 15 learnings spanning the full funnel from rescue surface → creative → download → retention. The original Apple Mail Rescue proved the concept (+55.7K DAU [038]), and the team has systematically scaled through creative optimization (Lottie [017], spam-fighting [020]), friction reduction (remove "Maybe Later" [018]), funnel optimization (v2.5 bottom sheet [054]), and surface expansion (Gmail [055], desktop [056]). The logout program [012] adds a compounding re-acquisition channel. Combined, these experiments represent the largest measured growth engine in the portfolio.

## Confidence-Ranked Findings

**High Confidence:**
- Apple Mail IMAP-Out Rescue 1: +55,700 DAU — the foundational experiment that proved the concept [038]
- IMAP-Out-Only logout: 6% yield, sustained, exceeded 2026 estimates by 50% [012]
- O&O + IMAP-Out users yield only 2.5% with significant leakage [013]
- Creative optimizations compound: Lottie (+5.7% Android) [017], spam-fighting (+22%) [020], removing "Maybe Later" (+16%) [018] — together scaled downloads from ~5K to 24K+/day
- Apple Mail Rescue 2.5: +24% downloads via bottom sheet UX [054]
- D30 retention: 17% Android, 11% iOS [027]
- Animation optimizations work better on Android: +6.4% on Android Gmail, flat on iOS Gmail [063]

**Medium Confidence:**
- Gmail IMAP-Out Rescue: ~1,780 downloads/day (70% Android, 30% iOS) — lower volume than Apple Mail but incremental [055]
- Desktop IMAP-Out Rescue: 100 iPad downloads/day + 1,000 desktop DAU — small but validates the concept on a new surface [056]
- Landshark DbS Animation: +18-19% downloads but paused due to revenue impact — captures the tension between acquisition and current-session revenue [057]
- Samsung Mail rescue terminated — Samsung blocks deep links at IMAP-in screen [sheet data]
- iPhone 17 launch spike: external events create download windows [028]
- New IMAP-Out surfaces (password screen toast) have very low CTR (0.05%) but high install rate (33.3%) among clickers [002]

## Contradictions
- **Removing friction helps in IMAP-Out** (remove "Maybe Later": +16% [018]) but **not in engagement features** (infinite scroll, auto subject lines [014, 003]). Hypothesis: friction removal works when blocking a high-intent action (app download) but not when motivation is absent.
- **Animations lift downloads on Android** (Lottie +5.7% [017], Gmail animation +6.4% [063]) but **are flat on iOS** [063]. The animation-as-persuasion mechanism may be platform-specific.
- **Landshark animations lift downloads 18-19%** [057] but **were paused for revenue impact**. IMAP-Out Rescue doesn't have this tension because rescued users weren't generating Yahoo revenue in their third-party clients. Landshark targets mobile web users who ARE generating revenue.

## Open Questions
- What is the ceiling for IMAP-Out Rescue downloads? Is there a point where the addressable pool of third-party client users is exhausted?
- Can desktop IMAP-Out be scaled beyond 1,000 DAU, or is the desktop rescue inherently low-volume?
- What's the re-logout yield for the 40M+ pool of previously logged-out users?
- Can the Landshark revenue tension be resolved (e.g., targeting only low-revenue mobile web users)?
- Why do animations work on Android but not iOS in the rescue flow?

## Opportunity Areas
- **Retention as the next frontier**: Downloads are solved (24K+/day). D30 retention of 11-17% means a 1-2% improvement = +35K DAU [027]
- **Android creative optimization**: Animations consistently lift Android downloads; the playbook is: test creative variants, measure platform-specific impact, GA for Android even if iOS is flat
- **Surface expansion**: Gmail rescue is live but small; desktop rescue is nascent. Each new surface adds incremental volume at low marginal cost
- **Rescue → onboarding pipeline**: IMAP-Out Rescue Onboarding with Tidy Inbox is being tested to improve post-download engagement
- **Device launch planning**: iPhone 17 drove 105K downloads in 7 days [028]. Preparing optimized experiences around predictable device launches

## Related Learnings
[002, 012, 013, 017, 018, 019, 020, 027, 028, 038, 054, 055, 056, 057, 063]
