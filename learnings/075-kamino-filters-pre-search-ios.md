---
id: "075"
title: "Kamino Filters Pre-Search iOS — +0.24% Search Success"
date: 2024-11-01
source: "Read Write Search Squad MPU Decks, Sept-Nov 2024"
themes: [engagement-features, search, mobile, filters]
confidence: high
goal: "engagement"
---

## Hypothesis
Yahoo Mail users need more support in the pre-search process to find the search results that are most relevant to them. We know that these users employ key topics to narrow down their initial search query. By exposing Kamino filters (aka topics) as pills for Yahoo Mail search users as they type their search query, we expect to see a 1% lift in the successful search rate because we are providing a better, narrower search before the user hits enter.

## Test Design
- **Platform**: iOS
- **Bucket**: 16%, 0.25% MDE, 2 weeks
- **Metric**: Search success rate, empty results rate
- **Status**: GA in version 7.55 (planned 12/06)

## Outcome
- **+0.24% stats sig lift in search success rate**
- **-4.4% stats sig reduction in empty search results**
- **Purchases (Receipt and Order) had the most clicks in pre-search** (~12K), followed by Travel, Finance, and Apparel
- For the Search Results Page, the "ALL" filter had the most clicks (~10K)
- GA approved, shipping in 7.55

## Nuance
The +0.24% lift fell short of the 1% hypothesis but is still stats sig and meaningful at Yahoo Mail's scale. The -4.4% reduction in empty results is arguably the more impactful number — fewer dead-end searches means less user frustration.

The category usage data is strategically valuable: Purchases/Receipts/Orders dominating pre-search clicks reveals that **transaction email lookup is the #1 search use case**. This should inform the "Personalized Kamino Filters" follow-up (planned Q1 2025) — personalizing filter order based on individual usage patterns could significantly amplify the lift.

The "ALL" filter being most popular on the SRP suggests users want to see comprehensive results after initial filtering, confirming that pre-search filters work as *intent narrowing* rather than *result restriction*.

This pairs with Email Suggestions [076] as a complementary search enhancement — filters help before the query, suggestions help during the query.
