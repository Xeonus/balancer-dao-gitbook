---
description: How do i calculate my boost for liquidity incentives in a pool?
---

# Calculating my Boost

To calculate a users boost the process from the [Maximum Boost](maximum-boost.md) section will be used considering the veBAL holdings user has.&#x20;

First we must calculate the user's working supply:

![The minimum of the working supply limit and liquidity provided & staked equation defines a user's working supply](<../../../../.gitbook/assets/Screen Shot 2022-04-09 at 10.57.00 AM.png>)

This would mean the minimum or “non-boosted” supply a user could have is the following, assume no veBAL is owned.

![](<../../../../.gitbook/assets/Screen Shot 2022-04-09 at 10.22.23 AM.png>)

The boost a user receives is the the ratio of their working supply over the new total working supply, divided by the minimum case of their working supply entering a pool.&#x20;

![The total working supply will need to be pulled from the gauge contracts for these calculations](<../../../../.gitbook/assets/Screen Shot 2022-04-09 at 11.08.51 AM.png>)

In the case of already being in the pool and depositing further liquidity, the following adjustment must to be made to consider the working supply a user already holds a given pool.&#x20;

![](<../../../../.gitbook/assets/Screen Shot 2022-04-09 at 11.28.35 AM.png>)
