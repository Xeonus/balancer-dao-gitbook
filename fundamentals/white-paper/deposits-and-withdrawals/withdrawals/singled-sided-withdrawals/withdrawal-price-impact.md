# Withdrawal Price Impact

Now let’s assume we are withdrawing from the BAL/WETH 80/20 Pool, we want to remove 5 WETH from the pool not knowing how many pool tokens we will need to redeem. We will be charged swap fees on the portion of our withdrawal which is “off-balance”. In this case 80% of our pool is not in the form of WETH, therefore that is the taxed portion. In this case we know we will receive the total of 5 WETH from the withdrawal, (At), this means our “sent” value will be unknown and slightly higher to compensate the swap fee we are charged.

The current pool traits are as follows:

* _**Swap fee: 0.05%**_
* _**BAL: 5,598,984**_
* _**WETH: 5,798.4836**_
* _**BPT: 2,816,401.77912812**_

![](<../../../../../.gitbook/assets/2 (4)>)

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-03 at 9.25.30 PM.png>)

This equation can be rearranged to solve for A (sent) in terms of our BPT (P\_redeemed) as follows:

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-03 at 9.25.45 PM.png>)

Using this equation, we can solve for A (sent):

For our Spot Price:

$$
A_{t}=B_{t} \ * \ \Bigg(1-\bigg(1-{\frac {P_{redeemed}}{P_{supply}}} \bigg)^{\frac {1}{W_{t}}} \Bigg)
$$

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-03 at 9.26.04 PM.png>)

From here we can calculate the amount of pool tokens we redeemed to receive our 5 WETH:

Then, we must calculate the ratio of the pool’s invariant before and after the withdrawal.

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-03 at 9.27.54 PM.png>)

Using the invariant ratio, we can determine the new total number of pool tokens and in the same stroke, calculate the amount of pool tokens needed to exchange for our WETH.

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-03 at 9.28.34 PM.png>)

Knowing the amount of BPT we needed to redeem and the amount of WETH we received in the withdrawal we can determine the effective price of a pool token to compare with our spot price:

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-03 at 9.29.08 PM.png>)

Please note the swap fee and pool traits change dynamically over time making calculations such as these valid for only a short period of time. The purpose of these examples is to deepen the understanding of our platform for those interested in are already utilizing Balancer Protocol.
