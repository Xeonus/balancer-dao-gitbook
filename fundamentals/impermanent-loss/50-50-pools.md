---
description: >-
  Examples will include impermanent loss calculations for a traditional AMM
  style pool (50/50) with swap fees or "APY" included.
---

# 50/50 Pools

We will start with a simple 50/50 pool featuring COMP/WETH. We take a time when WETH is worth $2,000 USD and we have 2.5 WETH ($5,000.00). At the same time COMP is worth $250.00 therefore we are investing 20 COMP tokens. Our liquidity position is deposited and we receive pool tokens for this $10,000 investment.

We check back out our position after a period of time and COMP has doubled, 100% gains straight to $500.00 USD. WETH has only made it up to $2300.00 at this point, gains of just 15%. We know at this point we will face some impermanent loss. We still have strictly gains but due to our liquidity position we are missing out on some of our investment in theory.

_Here we calculate the invariant from the value function:_

![](<../../.gitbook/assets/Screen Shot 2022-04-01 at 8.17.13 PM.png>)

![](<../../.gitbook/assets/Screen Shot 2022-04-01 at 8.16.16 PM.png>)

Here we can consider the USD values to be the same in the numerator and denominator therefore not needed to determine the ratio between the two.

![](<../../.gitbook/assets/Screen Shot 2022-04-01 at 8.17.57 PM.png>)

For the new token balances we consider the invariant ratio compared to the price action of the individual asset. This proportion will yield the new balance of each token in relation to the initial investment.

![](<../../.gitbook/assets/Screen Shot 2022-04-01 at 8.18.20 PM.png>)

_**Please note these calculations can take place over any time frame. These occurred in roughly 12 days between June 25 and July 07 of 2021. This same price action can take place over the course of 1 year and with 4% or more in swap fees or liquidity mining accumulating the LP position would become the more rewarding option.**_

These calculations are depicted by the following tables.

![](<../../.gitbook/assets/0 (1)>)

**Initial Investment: $10,000.00**

![](<../../.gitbook/assets/1 (6)>)

**HODL Total: $15750.00**

![](<../../.gitbook/assets/2 (2)>)

**LP Total $15165.75; with 4% Annual yield $15,772.38**

In our prior example COMP and WETH went through divergent price changes. When this happens, we saw the potential loss of value that can be created by the nature of impermanent loss. Now if our prices continue to change, we will look at an example where WETH goes up to a price of $3000.00 and COMP decreases down to $375.00. While these are diverging prices changes this will bring us to a 50% gain for both assets in relation to our original investment.

$$
V=20^{0.5}*2.5^{0.5}=7.071068 \\\ \\ V_2= (20*1.5)^{0.5}*(2.5*1.5)^{0.5}=10.6066017 \\\ \\ Invariant\ Ratio= {\frac {V_2}{V}}={\frac {10.6066017}{7.071068}}=1.5
$$

Therefore, because our invariant ratio matches our price action ratio, we have an indicator that there will be no impermanent loss.

![](<../../.gitbook/assets/Screen Shot 2022-04-01 at 8.20.07 PM.png>)

This calculation will be done from the point where impermanent loss was experienced to the current state to prove the “loss” is indeed reversible under the proper conditions.

**Initially:**

![](<../../.gitbook/assets/Screen Shot 2022-04-01 at 8.20.34 PM.png>)

**After Price Change:**

![](<../../.gitbook/assets/Screen Shot 2022-04-01 at 8.20.58 PM.png>)

New Token Balances can be calculated as follows:

$$
New\ Token\ Balances:B_{t'}*{\frac {Ratio_{LP}}{Price\ Action_t}} \\\ \\WETH:3.2969*{\frac {0.9890703}{1.30435}}=2.5 \\\ \\COMP: 15.16575*{\frac {0.9890703}{0.75}}=20
$$

These balances match our initial investment meaning overall we lost nothing impermanent loss. The price action is still in our favor by 50% for both assets as we hold the same initial number of each. Also, we would have likely earned swap fees for this from traders making our gains slightly larger.

Through the price action regardless of how dramatic impermanent loss can be reversed as seen above. This can occur countless times as prices of assets in a pool fluctuate in price. The importance of this is understanding the assets you are holding and how comfortable you are with volatility. In theory great volatility will be coupled with large volumes of trading making the swap fees and gains for liquidity providers increase. Weighing the risk of impermanent loss with the reward of accumulating swap fees or “volatility farming” is the game of a liquidity provider long term.
