# Trading Formulas

Balancer’s trade interface is based on several formulas which give a user the permissions to exchange tokens based on the relationships of the underlying pools. Balancer is host to many pools which contain the same tokens, creating the obstacle of which pool is best to route trades through. The solution is that we as users do not need to concern ourselves with deciding which pool to exchange with. While many tokens are found in several pools, Balancer has developed a Smart Order Router also known as the SOR. The SOR will guide a trade through all the options towards the one which benefits our traders the most.

Why would understanding Balancer Protocol’s trading formulas be important to a user? Every interaction with the Balancer Protocol will be impacted by these equations to some degree. For traders, understanding how the price of assets is calculated can vary across Automated Market Making Platforms. These equations are the foundation of market making on Balancer Protocol and create a massive potential for profitable use cases through arbitrage and liquidity provision. For liquidity providers these same equations will provide a gateway to earning swap fees and making long term positions earn yield by harvesting the surrounding market’s volatility.

Balancer’s formulas for trades as defined by the [whitepaper](https://balancer.fi/whitepaper.pdf) are the Out-Given-In, In-Given-Out, and the In-Given-Price which will be described below.&#x20;

The following variables will be used in these equations:

![](<../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.52.28 PM.png>)

Balancer Labs Documentation:

* [Swap Guides for Developers](https://dev.balancer.fi/guides/swaps)
* [Swaps Fees standard Math](https://docs.balancer.fi/concepts/fees)
* [Swap documentation for developers](https://dev.balancer.fi/resources/swaps)
* [Smart Order Router](https://docs.balancer.fi/products/smart-order-router)
