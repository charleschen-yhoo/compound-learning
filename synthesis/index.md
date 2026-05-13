# Synthesis Index

> This is a living document. It is rebuilt each time a new learning is added.
> Last updated: 2026-05-13
> Total learnings incorporated: 29

## Themes

1. **[IMAP-Out Rescue & Acquisition](imap-out-rescue.md)** — 10 learnings
2. **[Gamification & Engagement (Streaks/Challenges)](gamification-engagement.md)** — 11 learnings
3. **[Notifications](notifications.md)** — 3 learnings
4. **[Desktop vs Mobile Platform Dynamics](platform-dynamics.md)** — 5 learnings
5. **[Reactivation & Dormant Users](reactivation.md)** — 2 learnings
6. **[New Users & Activation](new-users.md)** — 1 learning

---

## Key Findings (Confidence-Ranked)

### High Confidence
- **Gamification disproportionately impacts less-active users.** Streaks v1, Challenges, and Streaks v2 all show the same pattern: Occasional and Tourist segments see 3-10x the engagement lift of Fanatics/Loyalists. This is the team's most consistent and replicable finding. [006, 007, 008, 025]
- **IMAP-Out-Only logout is a proven compounder.** 6% yield with no degradation over time, exceeded 2026 estimates by 50%. The most reliable growth lever the team has. [012, 013]
- **Creative and UX optimizations in IMAP-Out Rescue compound.** Lottie animations (+5.7% Android), spam-fighting creative (+22%), removing "Maybe Later" (+16%) — together these scaled daily downloads from ~5K to 24K+ over 12 months. [017, 018, 020]
- **Game mechanics drive exactly what they reward — nothing more.** Challenges only lifted stat sig on the actions that earn points (delete, read, open). Non-rewarded actions didn't move. [025]
- **Post-challenge/streak behavior persists.** Users don't just revert — O/T users maintain elevated DV7 after streaks end and PV lift persists after challenge windows close. [006, 008]

### Medium Confidence
- **Reducing friction doesn't always drive topline growth.** Auto subject lines and infinite scroll both improved the user experience without moving DV or revenue. Better UX ≠ more engagement. [003, 014]
- **Bulk delete is the strongest user value proposition.** Consistently the winning message in IMAP-Out Rescue, ad creatives, and direct feature usage (+9X actions with Cleanup Buddy). [005]
- **Performance optimization is a growth lever, not just tech debt.** Lottie animations delivered double-digit download lifts in emerging markets where device variability is high. [017]
- **Exit intent is the best moment for notification opt-in.** +0.58pp vs +0.22-0.53pp for other moments. Users leaving are most receptive to "stay connected." [016]
- **SMS is a cheap, positive-ROI reactivation channel.** $201 investment, $498 return, ROI-positive by Day 2. Platform shift from mobile web to iOS app over 45 days. [015]

### Emerging / Directional
- **Desktop features need active entry points.** Gamepad failed at 1.35% discovery. Desktop lacks push notifications as a re-engagement mechanism. [004]
- **Low-effort browser-level changes can move metrics.** Favicon update: +2.2% PVs with minimal dev effort. [023]
- **New user funnels are heterogeneous.** Gmail SIWG users vs new YMail users have different needs but weren't previously differentiated. [021]

---

## Contradictions & Open Questions

### Contradiction: Friction Reduction Impact
- **Removing "Maybe Later" increased downloads by 16%** [018] — removing a choice reduced friction and helped.
- **Auto Subject Lines had no engagement impact** [003] and **Infinite Scroll had no topline impact** [014] — removing friction didn't help.
- **Hypothesis for why:** The distinction is whether the friction is blocking a high-intent action (downloading an app you were prompted to get) vs. creating a low-friction path for an optional action (adding a subject line, scrolling to the next email). Friction removal works when users already want to act but are being impeded; it doesn't work when the underlying motivation is absent.

### Contradiction: O&O vs IMAP-Out-Only Logout Yield
- **IMAP-Out-Only:** 6% yield, sustained [012]
- **O&O + IMAP-Out:** 2.5% steady-state, significant leakage [013]
- **Hypothesis for why:** O&O users already have first-party access to Yahoo Mail. The logout is less disruptive — they have alternatives. IMAP-Out-Only users have no alternative, making the download compelling.

### Open Questions
1. **Will gamification impact plateau?** Streaks v1 → v2 → Challenges show consistent signal, but will users habituate and stop responding over time? The evergreen program (xPlatform Streaks) will be the test.
2. **What is the re-logout yield?** The 40M+ pool of previously-logged-out IMAP-Out users is being tapped, but steady-state yield for 2nd logouts is listed as "Unknown."
3. **Can SMS be automated at scale?** Legal/privacy compliance for automated transactional SMS is unresolved. If solved, this could become a significant automated reactivation channel.
4. **What drives the Android vs iOS retention gap?** D30 retention is 17% (Android) vs 11% (iOS) for IMAP-Out Rescue users. Root cause unclear — could be onboarding, user demographics, or platform behavior.
5. **Will relaxing challenge eligibility to 5+ emails deliver?** Hypothesis is strong (O/T users benefit most and have fewer emails) but hasn't been measured in production.

---

## Opportunity Areas

### 1. Notification Expansion (Desktop → Mobile → Cross-Platform)
Sticky notifications delivered +4,300 DAU on Windows alone. MacOS expansion expected to double this. 81% of users haven't opted in. Exit intent upsell is the best moment. There's a large, underexploited channel here. [001, 016, 026]

### 2. IMAP-Out Rescue Retention
Downloads are solved (24K+/day). Retention is the next frontier. D30 retention is 11-17% — a 1-2% improvement = +35K DAU. Onboarding experiments are underway. The volume makes even small retention gains massive. [027, 017, 018, 020]

### 3. Gamification Evergreen Program
Three experiments (Streaks v1, v2, Challenges) all confirm the thesis. O/T users respond dramatically. Post-treatment effects persist. The xPlatform Streaks program (2H'26) is the natural next step — making this permanent rather than experimental. [006, 007, 008, 025, 030]

### 4. Challenge Funnel Optimization
50% of users who hit Milestone 1 complete the full challenge. Getting more users to Milestone 1 is the highest-leverage optimization. Delaying opt-out (98% are Day 0) and relaxing eligibility (from 30+ to 5+ emails) are the two obvious levers. [009, 010, 011]

### 5. SMS Automation
Proven positive ROI at $0.003/message. Currently manual batch sends. Automating the campaign (Database → Evaluate → Telesign) would scale this channel. Legal approval for automated sends is the blocker. [015]

### 6. Desktop Engagement Surface Innovation
Desktop monetizes at ~10x less than mobile, but the user base is large. Favicon update (+2.2% PVs) shows low-effort browser-level changes can move metrics. Gamepad failed because of discoverability, not concept. Finding active entry points for desktop features is the challenge. [004, 023, 026]
