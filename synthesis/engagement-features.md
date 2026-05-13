# Engagement Features (Tidy Inbox, Default Mail, Sharing)

## Summary

Beyond gamification, the team has tested several engagement features that modify the core email experience. Tidy Inbox is the largest success here (+96.5K DAU on iOS [037]) but has shown diminishing returns in subsequent versions. Default Mail App is a one-time structural win (+28K DAU [041]). Email Sharing shows promise but has been blocked by product gaps. Cleanup Buddy works best when coupled with Tidy Inbox. The pattern: engagement features that help users manage existing email (triage, clean up) work; features that change how users use email (compose, share) are harder to land.

## Confidence-Ranked Findings

**High Confidence:**
- Tidy Inbox 1.5 (iOS): +96,510 DAU — the largest non-notification engagement experiment [037]
- Default Mail App (iOS): +28,000 DAU — a one-time structural setting that compounds [041]
- Tidy Inbox 1.6 (iOS): No DV lift — suggesting saturation on iOS after 1.5 [064]
- Infinite Scroll v2: No topline impact despite improved UX [014]

**Medium Confidence:**
- Tidy Inbox Android: engagement concentrated in Fanatic segment (1.5 iterated), eventually GA'd at +3,750 DAU in 1.6 [037, 052]
- Cleanup Buddy coupled with Tidy Inbox showed much stronger engagement than standalone [058]
- Email Sharing (iOS): +4,000 DAU but blocked by missing share retraction capability [051]

## Contradictions
- **Tidy Inbox 1.5 on iOS: massive success (+96.5K DAU)** vs **Tidy Inbox 1.5 on Android: only worked for Fanatics** [037]. Same feature, dramatically different segment response. On iOS, Tidy Inbox appeals broadly; on Android, only power users engage. This is the opposite of gamification [006, 008] where less-active users respond most.
- **Tidy Inbox 1.5 iOS: +96.5K DAU** vs **Tidy Inbox 1.6 iOS: zero lift** [037, 064]. The 1.5 version captured the addressable opportunity; 1.6 had nothing incremental to add. Diminishing returns set in fast.

## Open Questions
- Can Cleanup Buddy + Tidy Inbox coupling unlock DV lift, or is Tidy Inbox fundamentally a "try once" feature?
- Why does Tidy Inbox resonate broadly on iOS but only with Fanatics on Android?
- Is there a Default Mail App equivalent on Android (default email handler)?
- Can email sharing be unblocked by adding retraction capability?

## Related Learnings
[014, 037, 041, 051, 052, 058, 064]
