# In-Given-Price

_**In-Given-Price**_

Another approach or thought process that can be used between pools as opposed to increasing swap fees to make all pools equal in spot price, is the potential for arbitrage trading. Arbitrage trading is when a trader buys for example the excess BAL from the 80/20 pool and then sells it to the open market. If a large enough gap in price exists, then this will become an efficient transaction, after fees including gas payments are considered. Therefore, an arbitrager can make a profit by balancing out the spot prices of two sources.

The formula for the number of tokens traded to create the intended shift of this type of trading is defined in our [whitepaper](https://balancer.fi/whitepaper.pdf). A very important note here is the assumption that market depth is infinite for the new spot price. This will be elaborated on throughout the example.

In-Given-Price formula:

$$
A_{i} = B_{i} \ * \ \Bigg( \bigg({\frac {SP_{i}^{'o}}{SP_{i}^{o}}} \bigg)^{\frac {W_{o}}{W_{o}+W_{i}}}-1 \Bigg)
$$

The additional variables are defined as follows:

![](<../../../../.gitbook/assets/Screen Shot 2022-04-01 at 8.00.04 PM.png>)

For a further description on Spot Price and how it is calculated please refer to [The Value Function](../../the-value-function/) and [Spot Price](../../spot-and-effective-price/) sections of our documentation.
