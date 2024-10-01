---
description: How USDe Reserves are Calculated
---

# Reserves

## Accounts

| Account                                                                                                     | Assets            | Chain |
| ----------------------------------------------------------------------------------------------------------- | ----------------- | ----- |
| <pre data-full-width="true"><code><strong>0xA284e606624e60d5e218cC2061bd85eD3E4f073f
</strong></code></pre> | sUSDe, USDe, USDT | ETH   |
| <pre><code>0x6656F9769ccD9cC88E3088e47E8a4f3215798af2
</code></pre>                                         | USDe, USDT        | ETH   |
| <pre><code><strong>0x77b3898979f3947D8BFc931E6b6389a99d6727a9
</strong></code></pre>                        | sUSDe, USDe       | ETH   |
| <pre><code>eth:0xA1203607eCa4d5fe43aDb362D3b5E201183A5948
</code></pre>                                     | sUSDe, USDe       | ETH   |

## Calculation

[Bamk.fi](https://bamk.fi) updates the market value of the reserves every 10 minutes.&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2024-06-25 at 13.09.09.png" alt=""><figcaption></figcaption></figure>

The reserves are denominated in US dollar equivalent and is made up of:

> \+ sUSDe balance\
> \+ sUSDe unstaking (cooldown) balance\
> \+ USDe balance\
> \+ USDT balance\
> \= Total Backing

The code for how we calculate this figure on the website can be found [here](https://github.com/bamkfi/bamkfi-landing/blob/a8321bbbea58a17738dd9e2b60fc206ce138749b/src/app/page.tsx#L250).

## sUSDe Details

NUSD is backed 1:1 with USDe in phase 1. The majority of this is held in the form of Staked USDe (sUSDe) which is how Ethena pays out their yield.&#x20;

sUSDe is currently priced at $1.083 each and this price increases over time as Ethena's protocol revenue accumulates in their staking contract. This means our sUSDe Reserves figure will increase slightly every day, reflecting the yield earned. You can read [further details](https://ethena-labs.gitbook.io/ethena-labs/solution-design/staking-usde) about how the yield for sUSDe is paid.

Holding sUSDe is the way Bamk.fi generates revenue.

## Redemptions

NUSD can be redeemed directly for USDe via Bamk.fi's [redeem tool](https://docs.bamk.fi/bamkfi/how-tos/redeemnusd).&#x20;

We chose to give users USDe instead of sUSDe in the redeem tool because it is the most intuitive to understand - 1 NUSD = 1 USDe.&#x20;

Also sUSDe is far less liquid than USDe and we expect arbitrage traders will be the most frequent user of the redeem tool.

However Ethena has a 7-day cooldown period to unstake sUSDe. We therefore maintain a ratio of 10% USDe to 90% sUSDe in our reserves to facilitate instant redemptions of NUSD for users.&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2024-06-21 at 23.37.48 2.png" alt=""><figcaption><p>Unstaking sUSDe has a 7-day cooldown period</p></figcaption></figure>

Due to Ethena's policy of restarting the cooldown if additional sUSDe is unstaked from the same address, we may in the future have multiple backing addresses to better provide liquidity for redemptions.

\
