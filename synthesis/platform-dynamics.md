# Desktop vs Mobile Platform Dynamics

## Summary

Desktop and mobile are fundamentally different environments for growth, but the gap is more nuanced than "mobile good, desktop bad." Desktop monetizes at ~10x less per user [026], lacks push notifications as a re-engagement mechanism, and has discoverability problems [004]. However, desktop web notifications have delivered the single largest experiment in the corpus (+267K DAU [031]), and even low-effort changes (favicon) can move metrics [023]. A consistent cross-cutting finding: **Android and iOS respond differently to the same experiments**, with Android typically showing stronger response to creative/animation changes and more reliable GA rates for notification experiments.

## Confidence-Ranked Findings

**High Confidence:**
- Desktop per-user monetization is ~10x lower than mobile [026]
- Desktop web notifications launch: +267,000 DAU — proving desktop can deliver at massive scale with the right channel [031]
- Desktop features suffer from discoverability: Gamepad had 1.35% trial rate [004]
- Desktop lacks local notifications, which are the primary engagement driver on mobile [004]
- Animation/creative optimizations consistently work better on Android than iOS: Lottie (+5.7% Android [017]), Gmail rescue animation (+6.4% Android, flat iOS [063])

**Medium Confidence:**
- Low-effort browser-level changes can be surprisingly effective — favicon: +2.2% PVs, $3,398/day [023]
- The IMAP-Out → mobile app pipeline converts low-monetization desktop-adjacent users into high-monetization mobile users [026, 012]
- Android notification experiments GA more readily than iOS across multiple experiment types [046, 047, 039]
- Tidy Inbox works broadly on iOS but only for Fanatics on Android [037] — platform differences extend beyond monetization to feature engagement patterns

## Contradictions
- **Desktop delivered the #1 experiment** (web notifications: 267K DAU [031]) despite **desktop monetization being ~10x lower** [026]. The lesson: desktop's large user base means even low per-user impact can yield high absolute impact.
- **Engagement features work on desktop** (Challenges: +2.03% PV, sticky notifications: +4,300 DAU) but **Gamepad failed** [004]. The difference is entry points: features that are actively surfaced work; features that require discovery don't.
- **Same feature, different platform response**: Tidy Inbox broad on iOS, Fanatics-only on Android [037]. Gamification strongest for O/T on both [006, 008]. Notification nudges GA on Android, iterate on iOS [046]. There's no single "Android vs iOS" story — it depends on the feature type.

## Open Questions
- Are there other low-effort browser chrome optimizations (tab title, badge count) that could replicate the favicon effect?
- Should desktop engagement features be held to a different ROI threshold given the monetization gap?
- Can desktop web notifications partially substitute for mobile push as a re-engagement mechanism?
- Why do animations persuade Android users more than iOS users?
- Is the iOS/Android difference in notification experiment success rate due to platform UX, user demographics, or Apple's permission system?

## Related Learnings
[004, 014, 023, 026, 031, 037, 039, 046, 063]
