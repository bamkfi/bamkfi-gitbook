---
description: The four distinct stages of NUSD
---

# NUSD Issuance Primer

[Bamk.fi](http://bamk.fi) is the oldest and largest synthetic dollar protocol on Bitcoin, issuing the Nakamoto Dollar, _NUSD_.&#x20;

NUSD cycles through four distinct stages:

1. Pre-mined
2. Authorised&#x20;
3. Issued
4. Redeemed&#x20;

This article explains each of these stages and the associated onchain addresses users can publicly verify against.&#x20;

### Pre-mined

The majority of NUSD in circulation today is issued as [NUSD•NUSD•NUSD•NUSD](https://unisat.io/runes/detail/NUSD%E2%80%A2NUSD%E2%80%A2NUSD%E2%80%A2NUSD) on the Runes protocol. Due to limitations with the Runes protocol, the deployer of a Runes token is not able to have sole power to mint or burn supply like on Ethereum with smart contracts.&#x20;

[Bamk.fi](http://bamk.fi) therefore chose a max supply of 2.1 quadrillion NUSD (2,100,000,000,000,000) that was 100% pre-mined and sent to Asigna multisig address:

{% hint style="info" %}
bc1pfuluvkjcgzjdzjy42k3djkaw8a96dune2arcedhcml2h5sea6fdse9dajg
{% endhint %}

This gave Bamk.fi a supply that was essentially infinite with sole control of the issuance of NUSD tokens.

Pre-mined NUSD held at this address are not considered issued or circulating, and are therefore not backed by the equivalent USDe or delta-neutral position.

### Authorised

Authorised NUSD are sent in large batches from the pre-mined NUSD to the following address:

{% hint style="success" %}
TBA
{% endhint %}

The reason for Authorised NUSD is twofold:

1. **To minimise how frequently** [**Bamk.fi**](http://bamk.fi) **signer’s need to interact with private keys**

The [Bamk.fi](http://bamk.fi) Pre-mine address controls the ability for newly issued NUSD to circulate, so security of this address is our top concern. By issuing new NUSD in large batches we can greatly reduce how often private keys need to be used.&#x20;

2. **To meet customer demand at larger scale**

Secondly, maintaining an inventory of Authorised NUSD allows us to scale operations and meet customer demand in a timely fashion. The authorisation process ensures that NUSD won’t need to be issued every time a new customer request is made. Instead, a balance of Authorised NUSD is kept ready to be issued when needed without having to touch the private keys for the Pre-mine NUSD. The balance of Authorised NUSD is determined by conversations Bamk.fi has had with clients and represents the anticipated demand for NUSD.

Authorised NUSD are not yet issued and not in circulation, so they are therefore not backed by the equivalent USDe or delta-neutral position and not counted in the market cap of NUSD.

All authorised NUSD are held in [Bamk.fi](http://bamk.fi)’s treasury at the address(es) stated above and will not qualify for BAMK•OF•NAKAMOTO•DOLLAR rewards.

### Issued

Issued NUSD tokens are in circulation and fully backed by sUSDe, USDe or USDT. A breakdown of the reserves can be seen [here](https://docs.bamk.fi/bamkfi/resources/reserves).

In order to provide liquidity for BTC/NUSD swaps, Issued NUSD may be temporarily backed by BTC for 10 to 90 minutes while the protocol converts BTC to USDe/T.&#x20;

### Redeemed

Redeemed NUSD tokens are sent back to the Pre-mine address at `bc1pfuluvkjcgzjdzjy42k3djkaw8a96dune2arcedhcml2h5sea6fdse9dajg`. Clients who redeem NUSD will receive 1:1 amounts in either USDe or USDT, less any network fees.&#x20;

Once NUSD is sent back to the Pre-mined address they are no longer counted in the NUSD market cap.
