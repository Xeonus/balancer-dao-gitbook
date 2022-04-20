# Proportional Withdrawals

The opposite operation is needed to calculate the amount of each token remove from a pool upon withdrawing. The value we calculate will correlate to the balances of the tokens within the pool. Given any pool an investor may have funds in, they can determine the tokens they will receive as a % of the token balances.

Equation:

$$
A_{k}= \Bigg(1- {\frac {P_{supply}-P_{redeemed}}{P_{supply}}} \Bigg)* B_{k}
$$

The Balance term (Bk) will vary for every pool and each token within a pool however the portion of each balance an investor is entitled to is related to their share of the pool in reference to pool tokens always.&#x20;

As the external market prices of assets change the balances of tokens will fluctuate due to trading. The portion of the pool owned by an investor can only be changed as investors enter and exit the pool. For example, you may own 10% of a pool and after a few months as more people invest you now own 4% due to total supply of tokens increasing.

Assuming our previous example where we hold 1,500 pool tokens let’s assume the pool, we invested in has attracted far more liquidity. Now the total supply is at 25,000 pool tokens. Let’s calculate the number of tokens we will receive when we redeem our BPTs.

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-03 at 8.34.26 PM.png>)

Using the expression above we know that given the current balances of each asset in the pool (Bk) we will receive 6% of each token in our wallet upon redemption. These examples may be simple in nature but, coupled with swap fees, they are the first building block towards understanding the complexity of single of mixed asset deposits and withdrawals.
