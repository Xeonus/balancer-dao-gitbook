---
description: >-
  This is a proof for the net USD value of a pool based upon the invariant.
  Please note this can be done for any denomination of currency.
---

# Price Change Proof

The change in value of a Balancer pool given a price reference (in this case a base of USD) as seen on the medium article linked here can be defined by the following equation :&#x20;

![](<../../../.gitbook/assets/Screen Shot 2022-06-01 at 9.43.49 PM.png>)

Note per the whitepaper the invariant (V) is a constant value based upon a pool’s traits. This would mean that&#x20;

![](<../../../.gitbook/assets/Screen Shot 2022-06-01 at 9.43.54 PM.png>)

This understanding of the invariant as a constant surface is crucial when proving the initial equation stated to be true.&#x20;

1. Next, we can calculate the Value function in relation to the USD reference point using the following equations:

Assuming Pi is equal to the price of a token in reference to USD in this case

![](<../../../.gitbook/assets/Screen Shot 2022-06-01 at 9.51.17 PM.png>)

2\. Once a change in price occurs the Balance of each token will change due to the pool being rebalanced by arbitrageurs yielding (B’) at a new price (P’) in relation to the reference.&#x20;

![](<../../../.gitbook/assets/Screen Shot 2022-06-01 at 9.44.06 PM.png>)

3\. To determine the change in dollar value of our entire pool we will need the ratio of our new USD value divided by our initial USD dollar value. This is shown as the following:&#x20;

![](<../../../.gitbook/assets/Screen Shot 2022-06-01 at 9.44.11 PM.png>)

4.This is to be simplified to the following by isolating our balances from our prices.&#x20;

![](<../../../.gitbook/assets/Screen Shot 2022-06-01 at 9.54.32 PM.png>)

5\. Therefore the fraction of these two values is equal to 1 leaving:

![](<../../../.gitbook/assets/Screen Shot 2022-06-01 at 9.46.17 PM.png>)

![](<../../../.gitbook/assets/Screen Shot 2022-06-01 at 9.44.30 PM.png>)
