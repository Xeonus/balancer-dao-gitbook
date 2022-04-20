---
description: How to calculate the maximum boost possible and what effects it.
---

# Maximum Boost

Under certain conditions, specifically larger liquidity deposits, a maximum boost of less than 2.5x becomes apparent. The logic behind this is that there is only a finite number of incentives going to a pool, for example 10,000 BAL. Regardless of boosting, the pool's 10,000 BAL is distributed to the staked liquidity providers, boosting is a factor in which LP’s receive different portions of the incentives.

i.e. the pie is the same size but the slices are cut differently

The liquidity in terms of how much veBAL correlates to it what is called a working supply. The working supply can range from 40% to 100% of a user’s staked liquidity position. This is the main theory behind how rewards are distributed. The equation below defines a user’s working supply. (see variable list [here](minimum-vebal-for-max-boost.md))

![The minimum of the working supply limit and liquidity provided & staked equation defines a user's working supply](<../../../../.gitbook/assets/Screen Shot 2022-04-09 at 10.57.00 AM.png>)

This would mean the minimum or “non-boosted” supply a user could have is the following, assume no veBAL is owned.

![](<../../../../.gitbook/assets/Screen Shot 2022-04-09 at 10.22.23 AM.png>)

In turn, the maximum working supply possible is defined as the following:

![This is also equivalent to the liquidity provided and staked (l)](<../../../../.gitbook/assets/Screen Shot 2022-04-09 at 10.23.10 AM.png>)

To determine the maximum boost possible for a pool we must compare a user’s non-boosted and maximum working supply to the working supply the pool already has in place.

The pool’s working supply is the sum of all the liquidity providers working supplies prior to the deposit of a new user’s working supply.

The maximum boost possible for a user will be the ratio of their portion of max working supply plus the pools total working supply, divided by their portion of minimum working supply plus the pools total working supply. Please note the pools total working supply used here is prior to the user’s deposit.

![The total working supply will need to be pulled from the gauge contracts for these calculations](<../../../../.gitbook/assets/Screen Shot 2022-04-09 at 10.27.33 AM.png>)

Please note if a user has a working supply in a pool already, this must be subtracted total working supply in both the numerator and denominator of the equation a shown below.&#x20;

![](<../../../../.gitbook/assets/Screen Shot 2022-04-09 at 10.38.14 AM.png>)
