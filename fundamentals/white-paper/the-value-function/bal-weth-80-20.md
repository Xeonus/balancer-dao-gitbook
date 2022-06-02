---
description: >-
  This page will discuss both the 80/20 pool mechanisms as well as how to
  correlate USD value to the balance of tokens with in a pool. The relationship
  is a function of the pool traits.
---

# BAL WETH 80/20

Pools with assets which are much more independent of one another such as BAL/WETH are subject to impermanent loss which we can model here or see the simulator linked [here](https://baller.netlify.app/). The invariant function does not depend on external market prices, only the balance of tokens and weightings within the pool. However, we can consider a pool’s USD value over time.&#x20;

At the time of writing the BAL/WETH 80/20 Pool holds&#x20;

* 5,532,476 BAL ($112,530,555)&#x20;
* 9,726.09 WETH ($28,160,135)

Therefore, the total balance is $140,690,690.

The expected balances:

![](<../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.42.39 PM.png>)

Therefore, a pool can go through a transition to hold slightly more WETH than anticipated and slightly less BAL. Yielding the following charts.

![](<../../../.gitbook/assets/Screen Shot 2022-06-01 at 10.09.04 PM.png>)

In this case we now know our weights will be constant based on the pool ratios.

In the prior example an opportunity for profit through arbitrage presents itself. A trader or investor can input their tokens valued higher than the open market does in terms of USD in order to extract value in by exchanging on an external market.

This example is done at a snapshot in time, but please understand there is much more working internally. Slippage, price impact, and gas fees must be considered when an arbitrager is acting to rebalance a pool and extract profit for doing so.

