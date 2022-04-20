---
description: >-
  Two examples of calculating price impact with the incorporation of swap fees
  in single asset deposit scenarios.
---

# Price Impact; 10,000 BAL

Now let’s assume we are depositing into the BAL/WETH 80/20 Pool with 10,000 BAL and no WETH. We will be charged swap fees on the portion of our investment which is “off-balance”. In this case 20% of our pool is not in the form of BAL, therefore that is the taxed portion. As referenced from the[ trading with swap fees section](../../../spot-and-effective-price/price-impact-with-swap-fees.md).

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-03 at 8.52.19 PM.png>)

The calculation follows as:

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-03 at 8.52.35 PM.png>)

The current pool traits are as follows:

* _**Swap fee: 0.05%**_
* _**BAL: 5,691,640**_
* _**WETH: 6,194.1921**_
* _**BPT: 2,891,789.44800306**_

Using the known amount for A(t) we can calculate the amount of pool tokens we will be issued for this deposit.\


![](<../../../../../.gitbook/assets/Screen Shot 2022-04-03 at 8.53.27 PM.png>)

We can see on the user interface completing this transaction will yield a price impact of 0.03% (0.18% for the larger interaction). What exactly does this mean for an investor? Well in short from price impact for trading we can note that the ratio between assets change as supply and demand shifts during an exchange. In this case we are essentially exchanging BAL for Pool tokens and in doing so Pool tokens are becoming more expensive in reference to BAL. This is a bit more complex than comparing prices of individual assets in a pool, but we will focus on the current example to start. The spot price of a pool token and effective price of a pool token are the variables we need to calculate to determine our price impact from an investment.

![10,000 BAL Price Impact](<../../../../../.gitbook/assets/0 (2)>) ![100,000 BAL Price Impact](<../../../../../.gitbook/assets/1 (5)>)

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-03 at 8.57.48 PM.png>)

Pool token spot price (Assume A(t) = 1 BAL):

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-03 at 8.56.08 PM.png>)

Next, we must calculate the ratio of the pool’s invariant before and after the exchange of 10,000 BAL.

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-03 at 8.56.23 PM.png>)

Using the invariant ratio, we can determine the new total number of pool tokens and in the same stroke, calculate the amount of pool tokens which we received for the exchange.

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-03 at 8.57.17 PM.png>)

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-03 at 8.57.35 PM.png>)

Knowing the amount of BAL, we needed to invest and the pool tokens we received in exchange we can determine the effective price of a pool token to compare with our spot price:

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-03 at 8.57.48 PM.png>)
