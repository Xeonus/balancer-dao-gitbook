# In-Given-Out

_**In-Given-Out**_

The In-Given-Out equation will be the opposite thought process as the Out-Given-In formula. The idea is a trader, you, or I, wants to receive a specific number of tokens and this equation will solve how many tokens need to trade into a pool to receive that amount out. Note the variables defined in the introduction have not changed.

$$
A_{i} = B_{i} \ * \ \Bigg(\bigg({\frac {B_{o}}{B_{o}-A_{o}}}\bigg)^{{\frac {W_{o}}{W_{i}}}}-1\Bigg)
$$

For example, we will determine which of two pools is best to trade USDC for WMATIC on Balancer’s Polygon network pools. We will examine the two following pools TEL/WMATIC/USDC 60/20/20 (0.2%) and the WMATIC/USDC/WETH/BAL 25/25/25/25 (0.25%) pools.

| Pool (Wo / Wi)  | USDC Balance (Bi) | WMATIC Balance (Bo) |
| --------------- | ----------------- | ------------------- |
| 60/**20/20**    | 107,244           | 56,164              |
| 25/25/**25/25** | 5,194,894         | 2,722,125           |

Firstly, let us see what it will cost us to receive 1000 WMATIC as the amount we know we want out of our trade.

TEL/USDC/WMATIC 60/20/20:

![](<../../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.57.30 PM.png>)

WMATIC/USDC/WETH/BAL 25/25/25/25:

![](<../../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.57.56 PM.png>)

In the case we will spend less using our second option to receive the same amount of WMATIC making it the more desirable pool for the SOR to route us through. Now let’s incorporate swap fees.

