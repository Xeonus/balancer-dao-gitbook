---
description: >-
  This example is meant to emphasizes how token weights will affect internal
  values of tokens. Please note for stable coins a Stable pool is preferred over
  a Weighted Pool.
---

# Basic Weighted Pool

On a small scale we can assume the sample pool starts out with $10.00 of each token in it essentially:

Balance (t) is the number of tokens, Balance (USD) is the Balance (t) times it’s respective USD value.

Weight is number of tokens over total tokens

![](<../../../.gitbook/assets/0 (5)>)

![](<../../../.gitbook/assets/Screen Shot 2022-02-27 at 1.26.37 PM.png>)

Now if a swap occurred where someone was able to take 5 DAI out and put 5 USDC into the pool we would have the following situation. The pool thinks the value of each token has changed.

![](<../../../.gitbook/assets/1 (1)>)

![](<../../../.gitbook/assets/Screen Shot 2022-02-27 at 1.27.51 PM.png>)

In both instances the value function holds true yielding essentially the equations below:&#x20;

![](<../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.34.47 PM.png>)

To summarize our previous example and take a step closer towards the full understanding of Balancer Protocol’s dynamic system we must apply our knowledge to a more realistic setting. The pool’s weights (Wt) as we saw will in theory remain constant and in turn the value of each token will be manipulated in the eyes of the pool. This will alter the balance (Bt).

In the prior example an opportunity for profit through arbitrage presents itself. A trader or investor can input their DAI valued at $2.00 or remove USDC for $0.67 in terms of the other tokens. This is a magnified example but please understand there is much more working internally in terms of slippage. Stable coins while a pool is very small may experience some off peg (variation from $1.00) situations but hardly ever to this degree.
