# Including Swap Fees

_**Out-Given-In**_

One may raise the point that Balancer pools have fixed or dynamic swap fees and can be controlled by the pool owner(s). Therefore, it is possible that the best pool will change if the swap fee is considered, and a trader receives less BAL by paying the swap fee. To take the swap fee into account we will plug in an alternative value (Ai’) for the amount in (Ai) variable in the

![](<../../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.54.18 PM.png>)

At the time of writing the swap fee for the 80/20 pool is 0.05% and the 50/50 pool’s is 0.1%. Clearly with a lower fee and already higher yield, the 80/20 pool will remain the best route for traders yielding the following:

![](<../../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.54.47 PM.png>)

However, an optimization for pool holders can be made to increase the swap fee to the point where their pool is just slightly more favorable for traders. In this case the trader gets the best deal still while the liquidity provider is optimizing the market in their favor. This is outside the scope of the Out-Given-In Equation as the amount in and out will be known values while the swap fee will be an unknown value. Here is how our equation would look if we were to solve for Swap Fee.

![](<../../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.56.06 PM.png>)

![](<../../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.56.38 PM.png>)

We can now solve for the maximum swap fee the BAL/WETH 80/20 pool could have had set. This maximum fee correlates to the value at which the Amount Out for the Amount In would be competitive with the market and maximize swap fees collected by liquidity providers. To do this we will back calculate the swap fee at which the 80/20 could have had by using the 50/50 pools benchmark for amount out. All values are the pool traits of the 80/20, only the amount of (Ao) will be based on the prior 50/50 pool calculations.

![](<../../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.55.27 PM.png>)

Please note this a dynamic circumstance and the swap fees should be optimized over a longer period. Once a swap is executed the optimal swap fee will change due to the price impact a pool undergoes caused by a swap. Furthermore, pools on every decentralized exchange are competing for rates with lower swap fees and varying liquidity depths. This example is meant to be an introduction to how liquidity depth, relative prices, and fees are related.
