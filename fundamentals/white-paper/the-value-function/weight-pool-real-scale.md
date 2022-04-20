# Weight Pool - Real Scale

_Please note this is an example in **weighted** terms. The actual stable pool has a more dynamic system under the hood on Balancer._

At time of creation our stable pool holds roughly 163 million USD. To be less precise on decimals we will say USDC is 55 million, USDT is 54.5 million, and DAI is 53.5 million. Now we will see how those values compare before and after a swap 1000 times larger than out prior example. Please note in this example we are ignoring slippage and swap fees which are incurred during a trade. You will notice on site under these conditions 1 Dai is worth more than 1 USDC but proportions will not seem exact. Later lessons will dig deeper into these functionalities of the underlying algorithms.

![](<../../../.gitbook/assets/Screen Shot 2022-02-27 at 1.40.49 PM.png>)

We can see our pools will keep the weighting constant from the previous two diagrams. This means the value of the token will dynamically change with the quantity of each token in the pool. Therefore, the weights will remain constant and we must solve for the value of each token. The question now becomes how much each token worth is.

* Weight (Wt) will be constant, in this case 1/3. This is set during the creation of the pool
* The balance (B(USD)) will be our pool value over the number of tokens in this case is calculated by:

![](<../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.36.23 PM.png>)

* We can now determine our value of each token.

![](<../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.36.50 PM.png>)

Therefore our final calculation for the value function will yield the following equation:

![](<../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.37.25 PM.png>)
