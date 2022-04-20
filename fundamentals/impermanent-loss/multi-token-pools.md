---
description: >-
  Balancer's multi-token pools are on of our unique features. Below is an
  example of how impermanent loss on one of these pools on the can occur.
  Inclusive of details on volatility and stable coins.
---

# Multi-token Pools

_**Advanced Example – Multi Token Pool**_

An example of a multi token pool and how impermanent loss would occur and then be reverted will be solved below. We will look at a polygon pool: 25% USDC, 25% WMATIC, 25% BAL, 25% WETH. Initially we will assume we invested $10,000 in USD evenly amongst the assets.

Initial Conditions:

![](<../../.gitbook/assets/Screen Shot 2022-04-01 at 8.23.49 PM.png>)

We will assume USDC stays at a constant value, BAL increase by 15% to $28.75, WMATIC decreases 4% to $1.20, and WETH increase 50% to $3750.00.

![](<../../.gitbook/assets/Screen Shot 2022-04-01 at 8.24.15 PM.png>)

New Token Balances can be calculated as follows:

![](<../../.gitbook/assets/Screen Shot 2022-04-01 at 8.24.44 PM.png>)

Due to a stable coin (USDC) being a portion of the pool impermanent loss is nearly inevitable unless all tokens return to their initial value at the time of investment. Therefore, the pool above and any pool with stables and non-stable assets an investor is concerned mostly with volatility and their profit to be made from swap fees or reward APY. Essentially investing in their confidence for this type of price pattern:

![One may invest in a pool where USDC and an asset (X) at 14.01 are present in mid-July. Then by the time the chart comes to an end the price is still 14.01 after going through stages of upward and downward price changes. This will yield an amount of swap fees to be collected as profit as well as 0% impermanent loss.](<../../.gitbook/assets/3 (1)>)

At any point where all prices revert to their initial investment arbitragers will bring the tokens back to their initial balances. With a stable token present this would mean no gains can be made without impermanent loss or swap fees being present. In turn the goal can be considered to have low IL and high swap or reward APY for a liquidity provider with these types of investments. Also, it can be viewed to manage exposure to volatile assets.

![](<../../.gitbook/assets/Screen Shot 2022-04-01 at 8.25.26 PM.png>)

![](<../../.gitbook/assets/Screen Shot 2022-04-01 at 8.25.58 PM.png>)
