# Delta Neutral Hedging

## Phase 1: USDe Backing

In order to bootstrap and accelerate our launch, Bamk.fi's NUSD is backed 1:1 by Ethena's USDe in phase 1 which uses a similar delta-neutral position as NUSD will use in Phase 2.

## Phase 2: Delta-Neutral Positions on Bitcoin

The delta-neutral positioning will move towards placement on on-chain perpetual swaps. We are carefully monitoring trading volumes and open interest of various perp DEXs on several blockchains.

Longer-term, the development of the [Nakamoto Index](nakamoto-index.md) will provide onchain prices not requiring any centralized third-party oracles and enable [onchain perpetual swaps](bitcoin-perpetual-swaps.md) on Bitcoin itself.

We expect over time DEX perps volume to exceed CEX perps volume by orders of magnitude, which will allow NUSD to grow to the size of the market without leaving Bitcoin.

Enabling positions directly on-chain means we mitigate the largest risk factor in the creation of synthetic dollars: centralized exchange custody risk.

This further enables all positions to be transparent to the world at all times. Users can see actual positions being opened or closed by the Bamk.fi protocol.

### What is a Delta-Neutral Position?

In finance, a delta-neutral portfolio means despite the assets you hold going up and down in price, your portfolio value remains the same.&#x20;

Easiest explained with an example:

> BTC/USD is trading at $100,000&#x20;
>
> Your portfolio holds $10,000 worth of BTC (\~0.093 BTC).
>
> You want to keep your portfolio delta-neutral so you open a BTC short position worth $10,000 on the perpetuals pair.
>
> Now whether BTC goes to $150,000 or $20,000, your portfolio will still remain valued at $10,000&#x20;

You are going both long and short in equal amounts, simultaneously. This in effect cancels both positions out so you remain neutral.

### Synthetic Dollar

The ability to keep your $10,000 BTC portfolio delta-neutral means you can take your same portfolio and use it as backing for $10,000 worth of synthetic dollars. This is what the Nakamoto Dollar (NUSD) is.

Bamk.fi receives BTC from users in exchange for NUSD. Bamk.fi then opens an equally sized position going short BTC on the perpetuals pair. This creates the delta-neutral position. Bamk.fi can then issue fresh NUSD and have it backed by the delta-neutral portfolio.

### Bitcoin Bond and the Funding Rate&#x20;

When a perpetuals position is opened, something called the funding rate dictates whether long positions are paying shorts, or whether short positions are paying longs.&#x20;

Historically, \~74% of the time, long positions are paying shorts. The amount they pay can vary a lot, from 5% to 150% APY, depending on market supply and demand.

To continue with the example above, when your portfolio of $10,000 BTC becomes delta-neutral, you will \~74% of the time be receiving a yield because of your $10,000 short perpetuals position.&#x20;

This means the issuance of Nakamoto Dollars comes with it's own native yield - the Bitcoin bond.

There are further nuances to this, when the [funding rate turns negative](https://bamkfi.gitbook.io/bamkfi-docs/roadmap/negative-funding-rate-mitigation) and short positions have to pay long positions. But with a reserve fund and careful risk management policies this can be mitigated.&#x20;

### Potential Advantages of a Synthetic Dollar over Custodial Stablecoins&#x20;

On-chain collateral and transparency: All backing (BTC + matching short perp) is visible and auditable in real time, removing "trust us" reserve risk.

Reduced custodial exposure: No reliance on commercial banks, T-bills, or Treasury repos; mitigates freeze or seizure concerns.

Censorship resistance: Minting, transferring, and redeeming happen entirely on crypto rails without centralized gatekeepers.

Native yield potential: Positive funding on the short-perp leg can generate an organic return (“Bitcoin bond”) rather than idle cash reserves.

24/7 liquidity & settlement: Operates continuously on-chain, avoiding banking hours and wire-transfer bottlenecks.

Scalable supply: Issuance grows with available BTC liquidity instead of fiat deposit caps or banking relationships.
