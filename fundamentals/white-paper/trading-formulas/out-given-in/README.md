# Out-Given-In

_**Out-Given-In**_

The first function we will examine is the Out-Given-In which is used to calculate what you will receive based on what you are willing to sell. For example, if you know you will sell or spend a given amount of a token, we can calculate what tokens you will receive in return. Hence what amount you will get out, given what amount you put in; based upon the traits of the pool the trade is routed through.

$$
A_{o}=B_{o} \ * \ \Bigg( \ 1-\bigg({\frac{B_{i}}{B{i}+A_{i}}}\bigg)^{\frac{W_{i}}{W_{o}}} \ \Bigg)
$$

Let’s look at a very common trade, we will consider trading WETH for BAL. We have intentions of trading 2.5 WETH for the maximum amount of BAL possible. We will look at two possible pools we can route through to mimic what the Smart Order Router is doing under the hood of the Balancer Protocol to make sure users receive the best possible deal.

The two pools we will consider are the 80/20 (0.05%) and 50/50 (0.1%) BAL/WETH pools. At the time of writing, they hold the following balances.

| Pool (Wo / Wi) | WETH Balance (Bi) | BAL Balance (Bo) |
| -------------- | ----------------- | ---------------- |
| 80/20          | 6,005.3009        | 5,315,514        |
| 50/50          | 135.9922          | 30,158           |

(Please note these are excluding swap fees)

First, we will calculate the amount out for the potential 80/20 pool interaction

![](<../../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.53.10 PM.png>)

Next, we will determine the amount of BAL we would receive if interacting with the 50/50 pool

![](<../../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.53.37 PM.png>)

We can see here the SOR would direct us to the 80/20 pool for our swap to be executed, because it benefits us as the user to receive as much BAL as possible. If another pool exists which would give the trader even more BAL, that route would be executed. See the Smart Order Router section for an example of trade optimization routing through multiple pools as opposed to one. Please note the example above would yield the optimal number of BAL for a user if the trade was routed through both pools depending on the gas price.&#x20;
