# Phase 1 - USDe Backing

In order to bootstrap and accelerate our launch, Bamkfi's NUSD is backed 1:1 by Ethena's USDe in phase 1. This is held as Staked USDe (sUSDe) in our multi-sig backing address:

> [0xA284e606624e60d5e218cC2061bd85eD3E4f073f](https://etherscan.io/address/0xA284e606624e60d5e218cC2061bd85eD3E4f073f#tokentxns)

Price of 1 sUSDe = $1.072

Enabling this bootstrap allows us to immediately start growing TVL in an organic way. Phase 1 reliance on Ethena will be temporary as we further build out the infrastructure to execute our delta-neutral hedging program.

The protocol in phase 1 is already generating revenue, approximately $600 per day, or $219,176 per year.

## First is First

Since the inception of Ordinals on Bitcoin the idea for a stablecoin has been regularly shared. Several teams have attempted to create one but the only functioning ones we have seen are built on BTC L2s.&#x20;

Bamkfi wanted to get the Nakamoto Dollar circulating on L1 as soon as possible. So we decided to bootstrap in this way.

## BRC20-5byte vs Runes

The initial choice to start $NUSD on BRC20-5byte was because the upgrade was specifically intended for stablecoin projects. Tickers could be deployed without a max supply and issuance was only possible from the holder of the deployer inscription.&#x20;

On Runes there is no option for an infinite supply ticker where the deployer can control the issuance. So it was decided to etch the NUSD•NUSD•NUSD•NUSD Rune with a supply of 2.1 quadrillion, matching the number of satoshis of Bitcoin.&#x20;

We are keeping updated on other Bitcoin L1 protocols and will assess whether to deploy NUSD on other protocols.
