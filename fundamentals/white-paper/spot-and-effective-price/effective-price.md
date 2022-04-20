---
description: >-
  Here a guide and example of how effective price is calculated will be shown
  below. Please reference prior portions of this section, trading formulas, or
  the whitepaper for references.
---

# Effective Price

Next, we will look at the Effective Price which in short will consider the impact on the price you are making on the tokens as you make a trade. Note investing in a pool if it is not of perfect proportion is using the same principle in calculating price impact. The white paper shows the following formula:

$$
EP_{i}^{o}={\frac {A_{i}}{A_{o}}}
$$

* EP(i)^(o) represents the effective price of the token input in terms of the token output
* A(i) represents the number of tokens one will input (sell)
* A(o) represents the number of tokens one will output (buy)

This equation is not much use to us as we want to predict the effective price, and with the formula above we can only do this knowing the number of tokens we will get out of a trade. With the effective price increasing as we buy more of a token the above equation needs to be manipulated.

This brings us to the the Out-Given-In Function (see proof on [whitepaper](https://balancer.fi/whitepaper.pdf))

$$
A_{o}=B_{o} \ * \ \Bigg( \ 1-\bigg({\frac{B_{i}}{B{i}+A_{i}}}\bigg)^{\frac{W_{i}}{W_{o}}} \ \Bigg)
$$

Through substituting this equation into our Effective Price equation, we get the following relationship based strictly on variables which are known prior to a trade.

$$
EP_{i}^{o}={\frac {A_{i}}{B_{o} \ * \ \Bigg( \ 1-\bigg({\frac{B_{i}}{B{i}+A_{i}}}\bigg)^{\frac{W_{i}}{W_{o}}} \ \Bigg) }}
$$

Example Calculations for (BAL WETH 60/40 on Arbitrum)

Known pool trait values:

![](<../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.47.17 PM.png>)

We are willing to trade 10 WETH in. We will determine how much BAL we will receive and what the price impact of our trade is. We well repeat this for 100 WETH to compare the results.

![](<../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.47.47 PM.png>)

With these known values we can solve our effective price equation.

![](<../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.48.15 PM.png>)

The same equation for 100 WETH yields the following:\


![](<../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.48.41 PM.png>)

Clearly much more WETH is needed to buy a single BAL token, this adds up and grows as the amount going into a trade does. The market is being moved by the trade (within the confines of the pool).

Using this information, we can now calculate the price impact based on ratio between the spot price and the effective price. In theory the spot price equals the effective price only for extremely small trades. _(See Balancer_ [_whitepaper_](https://balancer.fi/whitepaper.pdf)_)_
