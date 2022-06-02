---
description: >-
  The center building block for all Balancer Protocol pools and swaps stems from
  the value function. Learn more in this section.
---

# The Value Function

The invariant, or Value Function, of Balancer Weighted Pools is critical for maintaining pool value and fair swap prices. . This weighted constant product equation facilitates pools of assets with fluctuating prices with respect  to one another. Fluctuations inherently lead to price impact, which creates r arbitrage opportunities for rebalancing the pool to market price. Another consequence of this mechanism is impermanent loss, or divergence loss. What does this mean to a user and what is different between two token and multiple token pools? We will look at several examples to explain the differences.

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

Bt is the balance of the token but this is not to be confused with the universal cost of the token. The pool is only as aware of prices as its contents dictate. The market of traders are responsible for (and financially incentivised to) making the value match the rest of the market.

For general use:

$$
B_{t}=\# \ of \ different \ tokens \ in \ the \ pool
$$

The USD value of the balance of a given token within the pool is dependent upon an external definition of price, often supplied by CoinGecko:

$$
B_{t}=( \# \ of \ different \ tokens \ in \ the \ pool ) \ * \ (External \ Price \ of \ token)
$$

_Wt_

Wt is the weight of the token in the pool. If a pool is well balanced with market prices, the weight of a token corresponds to how much of the pool’s value is denominated in that token.
