---
description: How does a single sided deposit work?
---

# Single Sided Deposits

The pool tokens issued to a depositor of a single asset can be determined by utilizing the change in the value function (invariant) of the pool. As seen in the [whitepaper](https://balancer.fi/whitepaper.pdf) the ratio of the change in the value function will yield the number of tokens issued. This information will become even more important when discussing multi-asset deposits:

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-03 at 8.44.47 PM.png>)

This can be simplified for our purpose of a single sided deposit where all other tokens in a pool maintain constant balances. The token which we are investing into a pool will be denoted with the letter “t”. Amount in (At), Balance-In (Bt), Weight-In (Wt) and the pool token supply will be the variables in concern. When simplified the equation is as follows:

$$
P_{issued}=P_{supply} * \Bigg(\bigg(1+ {\frac {A_{t}}{B_{t}}} \bigg)^{W_{t}}-1 \Bigg)
$$
