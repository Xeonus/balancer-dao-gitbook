---
description: >-
  Frequently asked questions and their answers from and by the Balancer
  Community.
---

# veBAL FAQ

**1. Will voters vote on how much emissions go to each network or is that locked?**

The voting mechanism is described in "How it works" in [Gauge voting documentation.](financial-implications/gauge-voting.md)

Voters will determine the amount of emissions going to gauge listed pools on each chain (Mainnet, Polygon, and Arbitrum), the voting will happen on mainnet. This is because the contracts to read your veBAL balance are on mainnet only.&#x20;

**2. If you have veBAL on mainnet, does it boost your farming on Arbitrum, Polygon?**

No, only gauges on L1 (Ethereum mainnet) receive incentive boosts because the contracts must read your veBAL balance.&#x20;

The boost depends on what fraction of the gauge staked liquidity you hold and what fraction of the total veBAL you hold. See more on boosting [here.](financial-implications/boosting-bal-incentives/)

**3. Is the veBAL vote on-chain,  and does it require gas fees?**

Yes, gauge votes are on-chain and cost a fee, when gas was 50 GWEI it was about $40 to vote, depending voting incentives (known as bribing) there is potential to offset the cost of voting. ****&#x20;

If the same pools will be selected each week, no additional vote, transaction, or gas is needed. Users only have to vote once, unless they want to change their allocation.&#x20;

Gas price is subject to change based on the price of ether and network congestion. ****&#x20;

**4. In the transitioning to veBAL, will I personally need to do any migration from the current pool I have invested?**

On mainnet, yes if your LP pool is eligible for gauge voting, you have to stake your LP for incentives.

On Polygon and Arbitrum, not in the initial launch period, but you will need to stake them in the near future.

The only lock-up necessary is to lock the BAL 80 - ETH 20 LP to receive veBAL.

**5. Do veBAL holders receive a portion of the trading fees? How are the protocol fees paid?**

veBAL holders are receive protocol fees distributed in bbaUSD (Boosted Aave Stable Pool LP Tokens) see [Protocol Revenue Distribution](financial-implications/protocol-revenue-distribution.md).&#x20;

**6. Is there a way to view how much total veBAL there is?**

Yes that information is in the following link: [https://dune.xyz/balancerlabs/veBAL](https://dune.xyz/balancerlabs/veBAL)

**7. How do I make a pool eligible for gauge voting?**

Need to make a governance proposal, [https://forum.balancer.fi/c/vebal/13](https://forum.balancer.fi/c/vebal/13)

**8. How much BAL/WETH BPT do I stake to maximize my multiplier? What amount do you need to stake at 1 year to hit the 2.5x boost for liquidity incentives?**

The length of time locked corresponds to how much veBAL you'll get for your 80/20 BPT. Voting is 1 veBAL for a 52 week lock of 1 BPT. Where a one week lock of 1 BPT will give 1/52 veBAL. **** See further info [here. ](vote-escrowed-governance.md)

The LM boost is separate. Related to your share of the pool and share of veBAL. Range limited from 1-2.5x. This can be calculated on our [tools site](https://balancer-tools.web.app/boost) and the math is explained [here. ](financial-implications/boosting-bal-incentives/calculating-my-boost.md)

**9. How do i get veBAL, and can i transfer BPT or veBAL?**

You will need to have BAL tokens or WETH to invest in the BAL/WETH 80/20 pool. You can deposit a single asset, which will incur some price impact, or you can deposit both assets in the correct weights. You will receive BPT which you can then time lock [here](https://app.balancer.fi/#/vebal) to receive veBAL.&#x20;

Yes, you can transfer BPTs. Rewards will accrue in the wallet where they are held.&#x20;

veBAL is a non-standard ERC-20 token and cannot be transferred.&#x20;

**10. How do I extend my veBAL lock up?**&#x20;

Just go to the [veBAL site](https://app.balancer.fi/#/vebal), see  "Lock until" , click "+", choose the time desired, and confirm.

**11. Are incentives paid daily?**

Incentives on mainnet are now accrued each block. Protocol fees are distributed on a weekly basis.

**12. Does veBAL support Gnosis Safe?**

It's normal for vote escrowed (ve) systems to not allow arbitrary contracts to lock as otherwise it's easy to tokenize the ve tokens which defeats the point. Users can lock up veBAL from an EOA and delegate it to your gnosis safe to earn boosts. [Guide link.](financial-implications/boosting-bal-incentives/boost-delegation-for-contract-wallet.md)

**13. Is there a repository for the contract addresses of all the new staking contracts and veBAL contracts?**

Link to the veBAL contracts:

{% embed url="https://github.com/balancer-labs/balancer-v2-monorepo/tree/master/pkg/deployments#past-deployments" %}

_Special thank you to community contributor Cosme Fulanito and baller Joey Wong for putting together these questions and answers._&#x20;
