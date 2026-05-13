# Engagement Features (Tidy Inbox, Default Mail, Sharing, Read/Write/Search)

## Summary

This theme covers two related bodies of work. The **Growth Squad's** engagement features (Tidy Inbox, Default Mail, Sharing, Cleanup Buddy) focus on email management and structural settings. The **Read Write Search (RWS) Squad's** experiments target the three core email actions — reading, writing, and searching — measured against engagement metrics (quality opens, sends per DAU, search success rate) rather than DAU/revenue directly.

**Tidy Inbox** is the Growth Squad's largest engagement success (+96.5K DAU on iOS [037]) but shows diminishing returns in 1.6. **Lightweight reply mechanisms** are the RWS Squad's most consistent win — Quick Replies (+3.5% [077]), Emoji Reactions (+2.97% [072]), and Toolbar updates (+1.8% [078]) all lift reply behavior on Android. **Search** improvements (Kamino Filters [075], Email Suggestions [076], Contact Filtering [079]) consistently improve search success. The emerging pattern: **reducing effort for actions users already want to take works; adding new capabilities users don't expect doesn't.**

## Confidence-Ranked Findings

**High Confidence:**
- Tidy Inbox 1.5 (iOS): +96,510 DAU — the largest non-notification engagement experiment [037]
- Default Mail App (iOS): +28,000 DAU — a one-time structural setting that compounds [041]
- Tidy Inbox 1.6 (iOS): No DV lift — suggesting saturation on iOS after 1.5 [064]
- Infinite Scroll v2: No topline impact despite improved UX [014]
- Quick Replies Android: +3.5% replies lift — GA'd [077 (engagement-measured)]
- Emoji Reactions Android: +2.97% replies lift, **no cannibalization** on toolbar replies or quick replies — these features are additive, not substitutive. ~20K DAU estimated, GA in 7.55 [072 (engagement-measured)]
- Email Suggestions iOS: removing suggestions = -2.76% search success — baseline validated, expanding to Android [076 (engagement-measured)]
- Message Read 2.5 Affiliate Revenue: +58.8% revenue, +95.29% clicks — reading improvements can serve revenue [080]
- Contact Search Filtering Desktop: +10K DAU — search improvements can drive business metrics [079]

**Medium Confidence:**
- Tidy Inbox Android: engagement concentrated in Fanatic segment (1.5 iterated), eventually GA'd at +3,750 DAU in 1.6 [037, 052]
- Cleanup Buddy coupled with Tidy Inbox showed much stronger engagement than standalone [058]
- Email Sharing (iOS): +4,000 DAU but blocked by missing share retraction capability [051]
- Kamino Filters Pre-Search iOS: +0.24% search success, -4.4% empty results — structured queries outperform free-text [075 (engagement-measured)]
- Message Read Toolbar Android: +1.8% replies lift — pure UX change, no new functionality needed [078 (engagement-measured)]
- Action Required Emails iOS: +14% opens, +22% CTR (orange variant) — directional but primary metric not yet significant [074 (engagement-measured)]
- Floating Compose Android: no lift in sends — FAB got +1% CTR (more compose taps) but control had highest compose-to-send conversion. Discoverability not the bottleneck; compose-to-send conversion is. Team pivoting to smart replies, auto-complete, AI compose for Q1 2025 [073 (engagement-measured)]

**Emerging / Directional:**
- Email sends per DAU declining YoY across all platforms (Android -2.9%, iOS -8.9%, Desktop -14.6%). Occasional users hardest hit (iOS -14.76%, Android -10.24%). Desktop decline partially from April instrumentation change. Team acknowledges "Quick Replies gains may not overtake send pattern loss." [071 (engagement-measured)]

## Key Patterns

### Writing: The Effort Reduction Thesis
Three Android experiments confirm that lowering the effort to reply drives engagement:
1. Quick Replies (+3.5% [077]) — AI-suggested responses
2. Emoji Reactions (+2.97% [072]) — one-tap reactions
3. Message Read Toolbar (+1.8% [078]) — better button placement

Meanwhile, Floating Compose (making compose *more visible*) failed [073] — the FAB generated more compose taps but *worse* compose-to-send conversion. Users don't need help *finding* compose — they need help *completing* the response. This reframes the "writing" problem as effort-reduction, not discoverability.

**Critically, these three features don't cannibalize each other.** The Emoji Reactions experiment confirmed no impact on toolbar reply or quick reply usage [072]. This means the combined lift from all three should be roughly additive, and the team can confidently ship all simultaneously.

### Reading: Classification Drives Action
Action Required Emails [074] shows that flagging emails needing action lifts opens (+14%) and CTR (+22%). Message Read 2.5 [080] shows that better presentation of commercial content lifts both engagement and revenue. The pattern: helping users *identify what matters* is more valuable than changing *how they read*.

### Search: Guardrails Beat Free-Text
Kamino Filters [075] (+0.24% success, -4.4% empty results) and Email Suggestions [076] (-2.76% when removed) both show that guiding users toward structured or suggested queries improves outcomes. Contact Search Filtering [079] (+10K DAU) proved this can translate to business metrics. **Mobile search hit 101% of goal** (62.62% vs 62% target) by November 2024, making search the RWS Squad's strongest pillar.

**Transaction email lookup is the #1 search use case**: Purchases (Receipts/Orders) had the most clicks (~12K) in Kamino pre-search, and Contacts had the highest CTR (18.44%) in email suggestions [075, 076]. Users primarily search to find specific emails from known senders about transactions.

## Contradictions
- **Tidy Inbox 1.5 on iOS: massive success (+96.5K DAU)** vs **Tidy Inbox 1.5 on Android: only worked for Fanatics** [037]. Same feature, dramatically different segment response.
- **Tidy Inbox 1.5 iOS: +96.5K DAU** vs **Tidy Inbox 1.6 iOS: zero lift** [037, 064]. Diminishing returns set in fast.
- **Reply mechanisms work on Android** (three positive experiments) but **compose discoverability didn't** [073]. Effort-reduction works; visibility doesn't.
- **Sends per DAU declining YoY** [071] despite **multiple GA'd features that lift send/reply metrics** [077, 078, 072]. The macro decline may be overpowering feature-level gains — or feature metrics (replies per user) and platform metrics (sends per DAU) measure different things.

## Open Questions
- Can Cleanup Buddy + Tidy Inbox coupling unlock DV lift, or is Tidy Inbox fundamentally a "try once" feature?
- Why does Tidy Inbox resonate broadly on iOS but only with Fanatics on Android?
- Is there a Default Mail App equivalent on Android (default email handler)?
- Can email sharing be unblocked by adding retraction capability?
- ~~Do Quick Replies, Emoji Reactions, and Toolbar improvements compound when all are live, or do they substitute?~~ **ANSWERED: They compound.** No cannibalization observed [072].
- Is the sends-per-DAU decline macro (industry-wide) or O&O-specific? IMAP-Out send data would answer this.
- Will iOS Quick Replies replicate Android's +3.5% lift?
- ~~Can search improvements (suggestions, filters) close the gap to the 62% mobile success rate goal?~~ **ANSWERED: Yes.** Mobile search at 62.62% (101% of goal) by November 2024.

## Related Learnings
[014, 037, 041, 051, 052, 058, 064, 071, 072, 073, 074, 075, 076, 077, 078, 079, 080]
