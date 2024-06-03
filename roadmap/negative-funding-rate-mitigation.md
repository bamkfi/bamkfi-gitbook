# Negative Funding Rate Mitigation

When phase 2 is live one of the biggest challenges will be what the Bamkfi protocol will do when funding rates are negative.&#x20;

Perpetual swaps work via a funding rate, which can either be positive or negative. When funding rate is positive, long positions are paying short positions. When funding rate is negative however, Bamkfi will be paying long positions to keep its short positions opened.&#x20;

Alongside a reserve fund to weather these periods of negative funding, Bamkfi will introduce these two policies depending on whether funding is positive or negative.

## Funding Rate Policies on Minting and Redemptions

* During positive rates on perpetuals, minting and redeeming are both open and BAMK rewards are given to holders of NUSD
* During negative rates on perpetuals, minting is suspended until rates are positive again, redeeming is open and BAMK rewards are given pro rata to redemptions per block

The above policy means NUSD TVL will remain dynamic based on market conditions, leading to greater resiliency. &#x20;



