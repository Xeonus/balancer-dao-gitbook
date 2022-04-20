---
description: >-
  This page will discuss both the 80/20 pool mechanisms as well as how to
  correlate USD value to the balance of tokens with in a pool. The relationship
  is a function of the pool traits.
---

# BAL WETH 80/20

Pools with assets which are much more independent of one another such as BAL/WETH are subject to impermanent loss which we can model here or see the simulator linked [here](https://baller.netlify.app).

In this case we now know our weights will be constant based on the pool ratios.

![](<../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.39.41 PM.png>)

Initial Market Prices: BAL $25.00 & WETH: $2200.00. We will invest $10,000 using “Best Price”.

![](<../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.40.06 PM.png>)

Shorthand $8000.00 in BAL, $2000.00 in WETH and our equation yield: 320 BAL and 0.909 WETH

To understand what we are expecting when we mint a pool token is to understand what we are really investing in. This is not the same as our balanced investments prior where each token is worth the same weight, so we experience an equation like this. (This is a bit more math intensive, but I will dissect.

Graphing the function on your own is recommended.

![](../../../.gitbook/assets/2) ![](<../../../.gitbook/assets/3 (4)>)

Essentially this chart is describing x\*y=k for variable weighted pools. This function is common knowledge as the constant for pooling interfaces across Defi. However, this typically is used for 50/50 style pool tokens.

In application the reciprocal of the function above is utilized to normalize investment values. In this case we know for our pool value of 80/20 we can determine the following.

![](<../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.40.35 PM.png>)

The reciprocal function is graphed below. This is a potential reference when debating what weights of tokens are desirable in terms of exposure to impermanent loss. Higher "y" values increase exposure to IL.    &#x20;

<img src="../../../.gitbook/assets/4 (1)" alt="" data-size="original">                       ![](../../../.gitbook/assets/5)

The above table shows shorthand estimations to incorporate the weighted token ratio into the value function to yield the actual dollar value of an investment.

Real time the BAL/WETH 80/20 Pool holds 5,532,476 BAL ($112,530,555) and 9,726.09 WETH ($28,160,135). Therefore, the total balance is $140,690,690.

The expected balances:

![](<../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.42.39 PM.png>)

Actual balances:

![](<../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.43.04 PM.png>)

Therefore, a pool can go through a transition to hold slightly more WETH than anticipated and slightly less BAL. Yielding the following charts.

![](<../../../.gitbook/assets/Screen Shot 2022-02-27 at 2.44.54 PM.png>)

In this case we will choose to rebalance this pool by exchanging our BAL for WETH. Assuming the prices of each asset are constant across our trade we can back solve for how much BAL needs to be exchanged for WETH in dollars to balance the pool.

The pool value should in turn remain constant given these constraints.

![](<../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.43.32 PM.png>)

Therefore, we can trade $21,997 BAL for WETH in the trade interface (assuming it is routed to the proper pool). Please note adding the single asset to the pool is not the same as the balance of WETH would not change in that case. This will be addressed can be addressed here (investment document link).

To double check this result as being correct we can use the interesting equation for value we learned earlier.

![](<../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.44.00 PM.png>)

This procedure must be done without rounding any decimal points to yield the exact answer. The larger the dollar values the more sensitive they are to small adjustments to decimals. This is good to note for financial literacy in terms of %’s of gains, losses, and relationships between different investment options. I look forward to discussing these dynamics further with you in future articles of Balancer White Paper Explained and a spin off I will write regarding Impermanent Loss. Until next time.

