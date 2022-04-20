---
description: >-
  An example of a calculation of spot price. Please see the intro for a
  reference to the equation used for spot price.
---

# Spot Price

See introduction [here](./)

Let’s look at an entry level example to understand Spot Price before moving on.

Assume a new pool is created. It is an 80/20 AAVE/WETH pool. The fair market price per CoinMarketCap is $284.00 per AAVE and $3500.00 per WETH. The pool creator started the pool off with 100k perfectly split in liquidity therefore we have 80k in AAVE and 20k in WETH.

![](<../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.44.59 PM.png>)

The relationship between the two can be described as:

![](<../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.45.29 PM.png>)

![](<../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.46.16 PM.png>)

Note: These values are precisely equal when using exact numbers. Small margins of error occur in above calculations due to rounding off to 4 or less decimal places.

That is how spot price works. The USD value is to be incorporated after the token relationship is determined in order to not overcomplicate the process the last step should be this conversion.
