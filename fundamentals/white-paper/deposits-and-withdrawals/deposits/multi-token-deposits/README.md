---
description: >-
  Multi-token deposits encompass the single sided deposit knowledge base and
  emphasize how Balancer Protocol's invariant and swap fees are incorporated in
  complex scenarios.
---

# Multi-token Deposits

Balancer Protocol has several features which differentiate it from all other core AMM platforms such as Uniswap and Curve. The one of focus in this section is the multi-token pools and the layer of complexity they add to the calculation of price impact, and ultimately disproportionate asset deposits.

Withdrawals only support proportional or single sided options in the current state; therefore, a single sided example will be solved. The principles defined in the proportional and single sided sections will be building blocks for the examples solved here.

For both examples we will utilize the WMATIC MTA WETH 40/40/20 Pool on Polygon as it highlights uneven weightings of assets as well as the multi-token aspects, we are interested in.
