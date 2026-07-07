# Negative Funding Rate Mitigation

When phase 2 is live one of the biggest challenges will be what the Bamk.fi protocol will do when funding rates are negative.&#x20;

Perpetual swaps work via a funding rate, which can either be positive or negative. When funding rate is positive, long positions are paying short positions. When funding rate is negative however, Bamk.fi will be paying long positions to keep its short positions opened.&#x20;

Alongside a reserve fund to weather these periods of negative funding, Bamk.fi will introduce these two policies depending on whether funding is positive or negative.

## Funding Rate Policies on Minting and Redemptions

* During positive rates on perpetuals, minting and redeeming are both open
* During negative rates on perpetuals, minting is suspended until rates are positive again, and redeeming is open

The above policy means NUSD TVL will remain dynamic based on market conditions, leading to greater resiliency. &#x20;



