---
description: This example is based upon the Arbitrum Weighted pool named in the title
---

# USDC WETH WBTC 33/33/33

At time of writing, this pool holds roughly 10.261 million USD. To be less precise on decimals we will say the pool holds $3.410MM of USDC, $3.422MM of WETH, and $3.429MM of WBTC. Please note in this example we are ignoring price impact and swap fees which are incurred during a trade. To solidify the idea that a pool is its own market and is independent of the external prices, we can see here that the USD price of USDC is slightly under $1. These prices are dictated directly by token balances, and will only be arbitraged back to market price by external users if the extractable amount is greater than the “financial friction” (gas and swap fees) of the system.

![](<../../../.gitbook/assets/Screen Shot 2022-06-01 at 9.26.48 PM.png>)

We can see our pools will keep the weighting constant. This means the value of the token will dynamically change with the quantity of each token in the pool.

![](<../../../.gitbook/assets/Screen Shot 2022-06-01 at 9.30.56 PM.png>)

* Weight (Wt) will be constant, in this case each token’s weight is 33.33% of the pool. This is set during the creation of the pool
* The value V(usd)  will be our pool value over the number of tokens in this case is calculated by:

![](<../../../.gitbook/assets/Screen Shot 2022-06-01 at 9.25.03 PM.png>)

We can now determine our value of each token.

![](<../../../.gitbook/assets/Screen Shot 2022-06-01 at 9.24.52 PM.png>)

Using the expected value as a benchmark for what the pool would hold in a perfectly balanced state, we can generate the following data:

![](<../../../.gitbook/assets/Screen Shot 2022-06-01 at 9.24.43 PM.png>)

In both instances the value function holds true yielding essentially the equations below:

![](<../../../.gitbook/assets/Screen Shot 2022-06-01 at 9.24.29 PM.png>)
