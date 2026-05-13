# Synthesis Index

> This is a living document. It is rebuilt each time a new learning is added.
> Last updated: 2026-05-13
> Total learnings incorporated: 64

## Themes

1. **[Notifications](notifications.md)** — 22 learnings (split into [Mobile](notifications-mobile.md) + [Desktop](notifications-desktop.md))
2. **[IMAP-Out Rescue & Acquisition](imap-out-rescue.md)** — 15 learnings
3. **[Gamification & Engagement (Streaks/Challenges)](gamification-engagement.md)** — 12 learnings
4. **[Engagement Features (Tidy Inbox, Default Mail, Sharing)](engagement-features.md)** — 7 learnings
5. **[Reactivation & Dormant Users](reactivation.md)** — 6 learnings
6. **[Desktop vs Mobile Platform Dynamics](platform-dynamics.md)** — 9 learnings (cross-cutting)
7. **[New Users & Activation](new-users.md)** — 1 learning

---

## Key Findings (Confidence-Ranked)

### High Confidence

- **Notifications are the #1 growth lever.** The top 6 notification experiments account for ~1M+ measured DAU impact. The foundational web notifications desktop launch alone delivered +267K DAU [031]. Mobile notification infrastructure optimization: +170K [032]. Important email filtering: +166K [033]. Cooldown tuning: +119K [034]. Sender redesign: +106K [036]. Tidy Inbox 1.5: +96.5K [037]. [031-036, 037]

- **IMAP-Out Rescue is a proven compounding growth engine.** Apple Mail Rescue 1 proved the concept (+55.7K DAU [038]). Creative optimizations compound: Lottie (+5.7%), spam-fighting (+22%), removing "Maybe Later" (+16%) scaled downloads from 5K to 24K+/day. IMAP-Out-Only logout yields 6% sustained [012]. [012, 017, 018, 020, 038, 054]

- **Gamification disproportionately impacts less-active users.** Streaks v1, Challenges, and Streaks v2 all show the same pattern: O/T segments see 3-10x the engagement lift vs F/L. Most consistent and replicable finding. [006, 007, 008, 025]

- **Post-challenge/streak behavior persists.** Users don't revert — O/T users maintain elevated DV7 after streaks end and PV lift persists after challenge windows close. [006, 008]

- **Android and iOS respond differently to the same experiments.** Animations lift Android downloads but are flat on iOS [063]. Android notification experiments GA more readily [046, 047, 039]. Tidy Inbox works broadly on iOS but only for Fanatics on Android [037]. There's no single "Android vs iOS" story. [037, 039, 046, 047, 063]

- **Notification quality beats quantity.** Important email filtering: +166K DAU [033]. Sender identity: +106K [036]. Inbox refresh upsell (high frequency): terminated with DV decrease [059]. [033, 036, 059]

### Medium Confidence

- **Desktop can deliver at massive scale with the right channel** despite ~10x lower monetization [026]. Web notifications: +267K DAU [031]. But desktop features require active entry points — Gamepad failed at 1.35% discovery [004]. [004, 026, 031]

- **The notification opt-in upsell hierarchy is clear.** Message read (+0.74%) > exit intent (+0.35%) > inbox refresh (terminated). Effectiveness correlates with contextual relevance and inversely with frequency. [045, 050, 059]

- **Reducing friction doesn't always drive topline growth.** Works in IMAP-Out (remove "Maybe Later": +16% [018]) but not in engagement (auto subject lines [003], infinite scroll [014]). Friction removal works when blocking high-intent actions. [003, 014, 018]

- **Email reactivation campaigns show promise but haven't been scaled.** User resurrection: +113K DAU (paused [035]). Win-back: +19K DAU (terminated [043]). SMS is ROI-positive by Day 2 at $0.003/message [015]. [015, 035, 043]

- **INTL markets have significant notification headroom.** iOS INTL persistent upsell: +20K DAU [042]. Android INTL lapsed returner: +4.7K DAU + $63/day [049]. Non-EN importance filter turnoff: +29K DAU [040]. [040, 042, 049]

### Emerging / Directional

- **Tidy Inbox may be hitting diminishing returns on iOS.** 1.5 delivered +96.5K DAU but 1.6 showed zero lift [037, 064]. Cleanup Buddy coupling may be the next iteration. [058, 064]
- **Low-effort browser-level changes can move metrics.** Favicon update: +2.2% PVs, $3,398/day [023]
- **Landshark animations create an acquisition/revenue tension** — +18-19% downloads but paused for revenue impact [057]

---

## Contradictions & Open Questions

### Contradiction: Android vs iOS Experiment Success
- **Android experiments GA more readily**: nudges [046], lapsed returner [047], persistent reminder [048], actions on notifications [039]
- **iOS sometimes delivers larger absolute impact**: notification redesign with sender +106K [036], Tidy Inbox 1.5 +96.5K [037]
- **Hypothesis:** Android's notification system is more permissive and users more responsive to iterative experiments. iOS has a higher bar (Apple permission system) but a larger addressable impact when cleared. Best practice: test on Android for faster signal, then iterate for iOS.

### Contradiction: Friction Reduction Impact
- **Removing "Maybe Later" increased downloads by 16%** [018]
- **Auto Subject Lines had no engagement impact** [003] and **Infinite Scroll had no topline impact** [014]
- **Hypothesis:** Friction removal works when users already want to act but are being impeded (high-intent); it doesn't work when the underlying motivation is absent.

### Contradiction: O&O vs IMAP-Out-Only Logout Yield
- **IMAP-Out-Only:** 6% yield, sustained [012]
- **O&O + IMAP-Out:** 2.5% steady-state, significant leakage [013]
- **Hypothesis:** O&O users have first-party alternatives; the logout is less disruptive for them.

### Contradiction: Notification Upsell Frequency
- **Exit intent works** (+9,828 PVs/day [045]) and **message read works** (+57% notif opened [050])
- **Inbox refresh upsell failed** — DV decrease, user complaints [059]
- **Hypothesis:** Upsell timing must match user intent, not just user presence. Once-per-session at meaningful moments (leaving, reading) is helpful; repeated during active use is intrusive.

### Contradiction: Tidy Inbox Platform Response
- **iOS Tidy Inbox 1.5: +96.5K DAU** (broad engagement) [037]
- **Android Tidy Inbox 1.5: only worked for Fanatics** [037]
- **Hypothesis:** iOS and Android users may have different email management habits, or the UX surfacing differs between platforms.

### Open Questions
1. **Will gamification impact plateau?** The evergreen xPlatform Streaks program (2H'26) will test this.
2. **What is the combined incremental DAU across all GA'd experiments?** Individual experiment DAUs may not be additive — need a holdback study.
3. **Can SMS be automated at scale?** Legal/privacy compliance is the blocker.
4. **Why were email campaigns (113K DAU, 19K DAU) not scaled?** Sustainability, retention, or cost concerns?
5. **What's the re-logout yield for the 40M+ previously logged-out users?**
6. **Can the importance classifier be retrained for non-EN languages?** [040]
7. **When will the service worker bug be fixed?** Two desktop notification experiments impacted [001, 060].

---

## Opportunity Areas

### 1. Notification Opt-In Waterfall (Desktop)
Layer the best-performing upsell moments in sequence: onboarding → message read → exit intent. Each captures a different user segment at a different intent level. 81% of users haven't opted in — this is the bottleneck. [016, 045, 050, 053]

### 2. IMAP-Out Retention
Downloads are solved (24K+/day). D30 retention of 11-17% means a 1-2% improvement = +35K DAU. Onboarding with Tidy Inbox is being tested. The volume makes even small retention gains massive. [027, 038]

### 3. INTL Notification Expansion
Non-EN users respond strongly to notification experiments when properly targeted: +29K DAU from turning off English-trained ML filter [040], +20K DAU from persistent upsell [042], +4.7K DAU + $63/day from lapsed returner [049]. INTL is an underinvested surface. [040, 042, 049]

### 4. Gamification Evergreen Program
Three experiments (Streaks v1, v2, Challenges) all confirm the thesis. O/T users respond dramatically. Post-treatment effects persist. xPlatform Streaks (2H'26) is the natural next step. [006, 007, 008, 025, 030]

### 5. MacOS Desktop Notification Expansion
Sticky notifications and reactivation notifications are Windows-only today. MacOS expansion should roughly double the addressable population and impact. Two experiments await the service worker bug fix. [001, 044, 060]

### 6. Challenge Funnel Optimization
50% of users who hit Milestone 1 complete the full challenge. Getting more users to Milestone 1 is the highest-leverage optimization. Delaying opt-out and relaxing eligibility are the two obvious levers. [009, 010, 011]

### 7. Android Creative Optimization Playbook
Animations consistently lift Android downloads (Lottie +5.7% [017], Gmail +6.4% [063], DbS +18-19% [057]) while being flat on iOS. This is a repeatable playbook: test creative variants, measure platform-specific impact, GA for Android even if iOS is flat. [017, 057, 063]

### 8. SMS Automation
Proven positive ROI at $0.003/message with natural mobile web → app migration. Currently manual. Automating the campaign would scale this channel. Legal approval for automated sends is the blocker. [015]
