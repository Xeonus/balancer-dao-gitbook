---
description: >-
  The center building block for all Balancer Protocol pools and swaps stems from
  the value function. Learn more in this section.
---

# The Value Function

The base component of balancer pools is based on the function below being true at all times. Due to this function, the pools which liquidity is stored in are open to fluctuating prices of tokens in reference to one another. This inherently leads to slippage and allows for arbitrage opportunities to rebalance the pool. Indirectly this leads to impermanent loss as well. Let’s dissect this with some numbers for a small scale and large scale example to see the effects.

Value Function:

$$
V= \prod_{t}B_{t}^{W_{t}}
$$

Where

* _t_ ranges over the tokens in the pool
* _Bt_ is the balance of the token in the pool
* _Wt_ is the normalized weight of the token, such that the sum of all normalized weights is 1.

_t_

Essentially _t_ represents how many tokens there are in a pool. We will do even splits to start (33/33/33) and look at when we have uneven weights (80/20) afterwards.

_Bt_

_Bt_ is the balance of the token but this is not to be confused with the universal cost of the token. The pool is only as aware of prices as its contents dictate the market of traders around it then are responsible for making the value match the rest of the market.

For general use:

$$
B_{t}=\# \ of \ tokens \ in \ the \ pool
$$

For purpose is terms of USDC:

![](<../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.32.54 PM.png>)

_Wt_

_Wt_ is the weight of the token in the pool and is best explained in an example since it is dynamic and related to the balance discussed prior. Think of it as the weight at a given set of prices of each token.
