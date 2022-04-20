---
description: >-
  How to calculate the maximum boost possible for a given liquidity pool and
  investment, as well as the boost a user is entitled to.
---

# Minimum veBAL for Max Boost

The variables to consider when calculating veBAL incentives boosts are the following:

* The Liquidity you will provide and stake: l
* The staked liquidity in the pool before you deposit and stake: L
* The liquidity in the pool after your deposit and stake: L' = L + l
* The total veBAL in circulation
* The amount of veBAL you hold

A common question is what is the minimum number of veBAL a user needs to hold in order to receive the maximum boost. To calculate this value:

![](<../../../../.gitbook/assets/Screen Shot 2022-04-09 at 10.15.38 AM.png>)

While this does answer what the minimum amount of veBAL is need for maximum boost at one point in time, we must consider what happens over time. if a user has the minimum veBAL required to receive maximum rewards and then more veBAL is minted, this means I will no longer be receiving the maximum rewards due to dilution of the Total veBAL.

To the opposite point, as more liquidity enters the pool your boost may increase, but net rewards decrease, while this is less critical one may require less veBAL if the portion of the pool they own decreases. Therefore, it is up to the user’s discretion how much veBAL they would like to hold.

See here how to calculate the [maximum boost](maximum-boost.md) one can receive from an investment.
