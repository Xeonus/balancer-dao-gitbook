# Proportional Deposits

Proportional deposits will yield newly minted Balancer Pool Tokens (BPT) for an investor. This function essentially states that the if the proportional amounts of all tokens deposited (Dk) in relation to the Balance of that given token (Bk) will yield that amount of the new total supply of pool tokens. The example in the whitepaper states that depositing 10% of each of the existing tokens in the pool an investor will receive 10% of the current BPT supply.

Equation:

$$
D_{k}= \Bigg({\frac {P_{supply}+P_{issued}}{P_{supply}}}-1\Bigg)*B_{k}
$$

Sample calculation:

Arbitrarily we will assume we are depositing 15% of the total balance meaning Dk divided by Bk will be 0.15

$$
{\frac {D_{k}}{B_{k}}}= 0.15 \ when \ deposit \ is \ 15\% \ of \ balance
$$

We will assume our total supply to be 10,000 BPTs at this time for the sake of simplicity. From here can make the following calculations:

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-03 at 8.29.58 PM.png>)

Substituting 0.15 for our deposit over balance ratio and 10,000 for the supply value we can solve for the issued amount of pool tokens.

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-03 at 8.31.30 PM.png>)

This shows that using the formula, based upon the number of tokens we deposit into a pool based upon the balance already we present we will be awarded a proportional number of pool tokens. These pool tokens are a user’s way to redeem their assets when the pool is exited.
