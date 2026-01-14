# Marketplace advertising position monitoring system

## Business background

Marketplace sellers heavily rely on internal marketplace advertising as their primary growth channel.
In most marketplaces, advertising works as an auction: sellers increase bids to secure top positions in search results for high-frequency and revenue-critical queries.

In theory, higher bids and active campaigns should guarantee stable visibility.
In practice, sellers often face unpredictable and opaque ranking behavior:

- Ads remain marked as active in the advertising dashboard;
- Impressions are still reported;
- But actual product visibility in search results suddenly drops or disappears

These drops may last from minutes to hours or even an entire day, directly impacting revenue while advertising costs continue to accrue.

## Problem statement

Existing marketplace analytics tools provide only low-frequency, aggregated metrics, such as average daily position, last observed position, a few scheduled measurements per day.

This approach hides short-term ranking failures, making it impossible to detect sudden ad suppression, understand real ad visibility dynamics and react in real time to revenue-critical issues.

As a result, sellers lose sales during visibility gaps, advertising budgets are wasted on ineffective impressions, operational decisions are made too late, when the damage is already done.

What sellers actually need is high-frequency, real-time position tracking, comparable to manual checks - but fully automated, scalable, and persistent.

## Key capabilities of the script

1. Real search result parsing

The script sends direct search requests to the marketplace search API and retrieves full product listings, iterates through search result pages, identifies the exact position of a target brand/product.

This allows detection of organic positions, promoted (ad) positions, complete disappearance from search results.

2. Multi-query and multi-region tracking

The system supports multiple search queries (including high-frequency keywords), multiple cities / regions (geo-dependent ranking behavior), brand-level filtering inside search results.

This reflects real marketplace behavior where rankings differ by query intent, user location and competition density.
