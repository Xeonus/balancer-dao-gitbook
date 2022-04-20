# Singled Sided Withdrawals

Single Sided Withdrawals will follow the same principles laid out in the single sided deposit section prior. The invariant is the core of these transactions and resulting equations are derived from there. As seen in the [whitepaper](https://balancer.fi/whitepaper.pdf) the ratio of the change in the value function will yield the number of tokens redeemed.

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-03 at 9.17.50 PM.png>)

This can be simplified for our purpose of a single sided withdrawal where all other tokens in a pool maintain constant balances. The token which we are removing from a pool will be denoted with the letter “t”. Amount Out (At), Balance-Out (Bt) before the transaction, Weight-Out (Wt) and the pool token supply will be the variables in concern. When simplified the equation is as follows:

$$
A_{t}=B_{t} \ * \ \Bigg(1-\bigg(1-{\frac {P_{redeemed}}{P_{supply}}} \bigg)^{\frac {1}{W_{t}}} \Bigg)
$$
