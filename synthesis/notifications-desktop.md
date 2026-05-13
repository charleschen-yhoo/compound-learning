# Desktop Web Notifications

## Summary

Desktop web notifications are an underexploited but rapidly maturing channel. The foundational launch [031] delivered +267K DAU — the single largest experiment in the entire corpus. Subsequent work has focused on (1) growing the opted-in base through contextual upsells [045, 050, 059], (2) improving notification quality [060, 061, 062], and (3) leveraging a unique capability: reaching logged-out users [044]. The key constraint is that 81% of desktop users haven't opted in [016], making opt-in growth the bottleneck for all other notification improvements.

## Confidence-Ranked Findings

**High Confidence:**
- Web notifications desktop launch: +267,000 DAU — the foundational experiment [031]
- Sticky important notifications: +4,300 DAU, +190.5% notif opens/user [001]
- Exit intent is the best opt-in moment: +0.35% opt-in rate, +9,828 PVs/day [045]; confirmed by earlier study at +0.58pp [016]
- Message read upsell: +0.74% opt-in, +57.26% notifications opened — users who opt in at this moment are highly engaged [050]
- Reactivation notifications bring back logged-out users: +10,435 PVs/day, +4% logged-out CTP [044]
- **Inbox refresh upsell failed** — DV decrease and user complaints. Too-frequent triggers cross from helpful to nagging [059]

**Medium Confidence:**
- 81% non-opted-in base represents a massive addressable pool [016]
- Rich notifications (sender icon): CTP increase with stats-sig but CTR only directional [061]
- Action buttons: same pattern as rich notifications — needs larger buckets [062]
- Sticky summary notifications: positive CTR/CTP but no PV lift, possibly due to service worker bug [060]

## Contradictions
- **Exit intent upsell works** [045] but **inbox refresh upsell hurts** [059]. Both are opt-in prompts on desktop. The difference: exit intent triggers once per session at departure (low frequency, high intent); inbox refresh triggers repeatedly during active use (high frequency, interruptive). Upsell timing must match user intent, not just user presence.
- **Sticky notifications boost engagement** [001, 060] but **don't always lift PVs**. Sticky summary notifications had positive CTR/CTP but no PV lift [060]. The difference may be urgency: "important email" creates urgency to click through; "summary" satisfies information need without requiring a click.

## Open Questions
- When will the service worker bug be fixed? Two experiments ([001], [060]) were impacted — clean reruns could show substantially higher PV impact
- MacOS expansion for sticky notifications: expected ~2x impact (Windows-only today) [001]
- Can the exit intent and message read upsells be combined in a waterfall? (Show message-read first since it has higher opt-in rate; fall back to exit intent)
- Can notification content be personalized to improve the 0.3% CTR baseline? [016]

## Opportunity Areas
- **Opt-in waterfall**: Layer the best-performing upsell moments — onboarding → message read → exit intent — to systematically grow the opted-in base
- **MacOS expansion**: Currently Windows-only for sticky notifications; doubling the surface should roughly double impact
- **Logged-out re-engagement**: Unique desktop capability [044] — no mobile equivalent. Could become a significant dormant user recovery channel
- **Rich notification + action button rerun**: Both showed positive CTP; larger buckets likely to confirm. This is incremental improvement on the 267K DAU base

## Related Learnings
[001, 016, 031, 044, 045, 050, 059, 060, 061, 062]
