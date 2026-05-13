# Mobile Push Notifications

## Summary

Mobile push notifications are the single largest DAU lever in the portfolio. The top 6 mobile notification experiments alone account for **~700K+ DAU** of measured impact. The team has systematically optimized across four dimensions: (1) delivery reliability [032], (2) content relevance [033, 036, 040], (3) frequency tuning [034], and (4) opt-in base growth [042, 046-049, 053]. A clear pattern emerges: Android experiments GA more readily and at higher scale than iOS, notification quality beats quantity, and INTL markets have significant untapped headroom.

## Confidence-Ranked Findings

**High Confidence:**
- Notification infrastructure optimization delivers massive returns: +170K DAU from network optimizations alone [032]
- Important email filtering on Android: +166K DAU — quality filtering > volume [033]
- Cooldown cadence tuning (7→5 days): +119K DAU from a parameter change [034]
- Notification redesign with sender identity: +106K DAU on iOS [036]
- Actions on notifications: +47.5K combined (Android +32.5K, iOS +15K) — Android 2x iOS [039]
- Turning off importance filtering for non-EN users: +29K DAU — ML model accuracy varies by language [040]
- Android consistently outperforms iOS for notification experiments: nudges (+9.1K Android GA vs iOS iterate [046]), lapsed returner (Android 3x iOS [047]), persistent reminder (comparable [048])

**Medium Confidence:**
- INTL markets have significant headroom: iOS INTL persistent upsell +20K DAU [042], Android INTL lapsed returner +4.7K DAU + $63/day revenue [049]
- Notification opt-in nudges require iteration — v1 terminated, v2 iterated, v2 rerun GA'd [046]
- Lapsed returner moment is an effective opt-in trigger across platforms and geographies [047, 049]
- Moving notification permission to position 1 in onboarding: +2.4K DAU on iOS (Android terminated) [053]

## Contradictions
- **Android experiments GA more readily** but **iOS sometimes delivers larger absolute impact** (sender redesign: 106K on iOS alone [036] vs typical Android notification experiments at 10-30K). The pattern isn't "Android > iOS" — it's "Android is more predictable, iOS is higher-variance."
- **Quality filtering helps EN users** [033] but **hurts non-EN users** [040]. The importance classifier's accuracy is language-dependent.

## Open Questions
- Can the cooldown be pushed further (5→3 days) or is there a fatigue cliff?
- What's the combined incremental DAU when all notification experiments are GA'd simultaneously? (Individual experiment DAUs may not be additive)
- Can the importance classifier be retrained for non-EN languages, or is the "turn off filtering" approach better?
- iOS lapsed returner INTL needed re-run — will it match Android's success?

## Related Learnings
[032, 033, 034, 036, 039, 040, 042, 046, 047, 048, 049, 053]
