# Notifications (Overview)

> **This theme has been split into two sub-themes due to scale (22+ learnings):**
> - **[Mobile Push Notifications](notifications-mobile.md)** — 12 learnings
> - **[Desktop Web Notifications](notifications-desktop.md)** — 10 learnings

## Cross-Platform Summary

Notifications are the single largest growth lever in the portfolio. The top experiments account for **~1M+ measured DAU impact** across mobile and desktop. The notification optimization stack follows a clear hierarchy:

1. **Delivery reliability** (infrastructure) — 170K DAU [032]
2. **Content relevance** (important filtering, sender identity) — 272K DAU [033, 036]
3. **Frequency tuning** (cooldown, cadence) — 119K DAU [034]
4. **Opt-in base growth** (upsells, nudges, onboarding) — 50K+ DAU [042, 046, 047, 048, 053]
5. **Notification UX** (sticky, actions, rich) — 50K+ DAU [001, 039]
6. **Re-engagement** (reactivation, logged-out) — 10K+ PVs/day [044]

## Key Cross-Platform Pattern

**Android notification experiments GA more reliably than iOS.** Across nudges [046], lapsed returner [047], persistent reminder [048], and actions [039], Android consistently outperforms. However, iOS can deliver larger absolute impact when it works (notification redesign with sender: +106K on iOS [036]). The implication: test on Android first for faster signal, then iterate for iOS.

## The Upsell Hierarchy (Desktop)

Not all opt-in moments are equal:
1. **Message read** — +0.74% opt-in (highest rate, contextually relevant) [050]
2. **Exit intent** — +0.35% opt-in (departure moment, low frequency) [045]
3. **Inbox refresh** — TERMINATED (too frequent, user complaints) [059]

The lesson: upsell effectiveness correlates with contextual relevance and inversely correlates with frequency.
