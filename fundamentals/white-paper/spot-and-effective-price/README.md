---
description: >-
  This section will outline spot price and effective price with the end goal of
  explaining how price impact, also known as slippage in some cases, is
  calculated.
---

# Spot & Effective Price

In order to understand how swaps are going to alter the price of tokens in a pool we must understand the relationship between the spot and effective prices tokens assign to one another as pools go on and off balance. In theory trades in any market are working with a mechanism of price impact. Supply and demand is the root logic, where as you take more of something out of circulation, it becomes more valuable. For example people consume more of a certain product, the price will go up because there is less of it. This happens in an extreme way when swapping a large amount of tokens. The value of what you want goes up, the value of what you are selling in turn will go down.

Dissecting the spot price and effective price functions followed by some small scale and real scale examples will bring us to understand price impact.

The Spot Price as defined in the Whitepaper:

$$
SP_{i}^{o}={\frac {\frac {B_{i}}{W_{i}}}{\frac {B_{o}}{W_{o}}}}
$$

Where the variables represent the following:

* SP(i^o) is the spot price of the input and output tokens in the pool.
* B(i) is the balance of the token coming into the pool (input)
* W(i) is the weight of the token coming into the pool (input)
* B(o) is the balance on the token going out of the pool (output)
* W(o) is the weight of the token going out of the pool (output)

Important to note that these variables are from a pool in a stagnant state. Do not incorporate the swap you are planning in to do by adding or subtracting the balance changes you will create in your swap at this point.

Balancer Labs Documentation:

* [Swaps Fees standard Math](https://docs.balancer.fi/concepts/fees)
* [Swap documentation for developers](https://dev.balancer.fi/resources/swaps)
* [Smart Order Router](https://docs.balancer.fi/products/smart-order-router)
