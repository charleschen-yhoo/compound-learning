# Desktop vs Mobile Platform Dynamics

## Summary

Desktop and mobile are fundamentally different environments for growth. Desktop monetizes at ~10x less per user, lacks push notifications as a re-engagement mechanism, and has a discoverability problem for new features. However, the desktop user base is large, and even low-effort changes (favicon) can move metrics. The strategic implication: initiatives that shift users from desktop to mobile (IMAP-Out Rescue) have outsized revenue impact; desktop engagement features need to be evaluated on a different ROI bar.

## Confidence-Ranked Findings

**High Confidence:**
- Desktop per-user monetization is ~10x lower than mobile [026]
- Desktop features suffer from discoverability problems — Gamepad had 1.35% trial rate with a passive entry point [004]
- Desktop lacks local notifications, which are the primary engagement driver for mobile features like Gamepad [004]

**Medium Confidence:**
- Low-effort browser-level changes can be surprisingly effective — favicon update: +2.2% PVs [023]
- The IMAP-Out → mobile app pipeline effectively converts low-monetization desktop-adjacent users into high-monetization mobile users [026, 012]

## Contradictions
- **Engagement features work on desktop** (Challenges: +2.03% PV, sticky notifications: +4,300 DAU) but **Gamepad failed**. The difference is entry points: Challenges and notifications are actively surfaced; Gamepad required users to discover it.

## Open Questions
- Are there other low-effort browser chrome optimizations (tab title, badge count, etc.) that could replicate the favicon effect?
- Should desktop engagement features be held to a different ROI threshold given the monetization gap?
- Can desktop web notifications partially substitute for mobile push notifications as a re-engagement mechanism?

## Related Learnings
[004, 014, 023, 026, 003]
