---
description: Via onchain perpetual swaps
---

# Phase 2 - Delta Neutral Hedging

In phase 2, we will start our hedging program. We have a trading firm we have worked with before who will help execute and manage the delta-neutral hedging program.

Bamkfi plans to execute the delta-neutral hedging program only through onchain perpetual swaps. We are carefully monitoring trading volumes and Open Interest of various perpetual DEXes on several blockchains.

Longer-term the development of the [Nakamoto Index](nakamoto-index.md) will provide onchain prices not requiring any centralized third-party oracles and enable [onchain perpetual swaps](bitcoin-perpetual-swaps.md) on Bitcoin itself.

We see onchain perps volume exceeding centralized exchange perp volume in the future by orders of magnitude.

Enabling hedging directly onchain means we mitigate the largest risk factor in the creation of synthetic dollars - centralized exchange custody risk.

## Delta-Neutral Position

In finance, a delta-neutral portfolio means despite the assets you hold going up and down in price, your portfolio value remains the same.&#x20;

Easiest explained with an example:

> <mark style="background-color:orange;">BTC/USD is trading at $69,000</mark>&#x20;
>
> <mark style="background-color:orange;">Your portfolio holds $10,000 worth of BTC (\~0.14492 BTC).</mark>
>
> <mark style="background-color:orange;">You want to keep your portfolio delta-neutral so you open a BTC short position worth $10,000 on the perpetuals pair.</mark>
>
> <mark style="background-color:orange;">Now whether BTC goes to $150,000 or $20,000, your portfolio will still remain valued at $10,000</mark>&#x20;

You are going both long and short in equal amounts, simultaneously. This in effect cancels both positions out so you remain neutral.

## Synthetic Dollar

The ability to keep your $10,000 BTC portfolio delta-neutral means you can take your same portfolio and use it as backing for $10,000 worth of synthetic dollars. This is what the Nakamoto Dollar (NUSD) is.

Bamkfi receives BTC from people who want to mint NUSD. Bamkfi then opens an equally sized position going short BTC on the perpetuals pair. This creates the delta-neutral position. Bamkfi can then issue fresh NUSD and have it be backed by the delta-neutral portfolio.

## Bitcoin Bond and the Funding Rate&#x20;

When a perpetuals position is opened, something called the funding rate dictates whether long positions are paying shorts, or whether short positions are paying longs.&#x20;

Over 74% of the time, long positions are paying shorts. The amount they pay can vary a lot, from 5% to 150% APY, depending on market supply and demand.

To continue with the example above, when your portfolio of $10,000 BTC becomes delta-neutral, you will 74% of the time be receiving a yield because of your $10,000 short perpetuals position.&#x20;

This means the issuance of Nakamoto Dollars comes with it's own native yield - the Bitcoin bond.

There are further nuances to this, when the [funding rate turns negative](https://bamkfi.gitbook.io/bamkfi-docs/roadmap/negative-funding-rate-mitigation) and short positions have to pay long positions. But with a reserve fund and careful risk management policies this can be mitigated.&#x20;

