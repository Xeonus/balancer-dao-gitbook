---
description: Key questions and answers to how boosting incentives works with veBAL system.
---

# Boosting BAL Incentives

As opposed to the initial liquidity mining incentives where a liquidity provider receives incentives based only on their share of the total liquidity, we will now implement a multiplier based upon the time locking mechanism. Locking the same amount of BPT for a longer period will yield a higher incentive multiplier for a user.

![](<../../../../.gitbook/assets/Screen Shot 2022-04-09 at 9.57.22 AM.png>)

Please note the maximum boost possible for liquidity mining incentives is 2.5x. See here how to [calculate your boost](calculating-my-boost.md).

The boosting mechanism theory is visualized by the graphic below. The fraction of a pool's working supply a user owns is based on upon their share of their respective pool, and their share of total veBAL. Continue reading through this boosting sections for further information on the working supply.

![](<../../../../.gitbook/assets/veBAL Boost Graphic 3.gif>) ![](<../../../../.gitbook/assets/Screen Shot 2022-04-16 at 4.42.04 PM.png>)

Based upon this new mechanism locking the same number of tokens for twice as long as someone else will result in twice the voting strength. The boosting proportion and more additional benefits are coupled with wielding that strength, however they are not as directly proportional.

_Special thank you to Baller, zekraken, for deconstructing the contracts & code to make calculating boost easily accessible to the Balancer community._&#x20;

_Reference link the_ [_boosting graphic_](https://www.desmos.com/calculator/d3mhco4zwx) _in more detail._&#x20;
