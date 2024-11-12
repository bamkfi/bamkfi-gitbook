---
description: The protocol holds assets in the following addresses.
---

# Reserves

## Accounts

| Account                                                                                                     | Assets                                     | Chain |
| ----------------------------------------------------------------------------------------------------------- | ------------------------------------------ | ----- |
| <pre data-full-width="true"><code><strong>0xA284e606624e60d5e218cC2061bd85eD3E4f073f
</strong></code></pre> | sUSDe, USDe, USDT                          | ETH   |
| <pre><code>0x6656F9769ccD9cC88E3088e47E8a4f3215798af2
</code></pre>                                         | USDe, USDT                                 | ETH   |
| <pre><code><strong>0x77b3898979f3947D8BFc931E6b6389a99d6727a9
</strong></code></pre>                        | sUSDe, USDe                                | ETH   |
| <pre><code>0xA1203607eCa4d5fe43aDb362D3b5E201183A5948
</code></pre>                                         | sUSDe, USDe                                | ETH   |
| <pre><code>0xD00a4c08349d5a82df98C606262AfC4ae2d8075D
</code></pre>                                         | sUSDe, USDe                                | ETH   |
| <pre><code>bc1prnqh4uznxaklvxga6spr2fyjrpcxwnryzlhdpghzq9zqgz59z54qmentw6
</code></pre>                     | BTC, NUSD (Authorized, Out of circulation) | BTC   |

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

\
