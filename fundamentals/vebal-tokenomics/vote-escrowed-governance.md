---
description: An overview of the redefined governance system for Balancer Protocol
---

# Vote-Escrowed Governance

veBAL is the newest pillar of Balancer’s governance system. Derived from Curve finance vote-escrowed voting essentially gives holders of a respective protocol’s token the ability to lock their asset for a period. The longer the asset is locked, the more voting strength their assets are delegated by escrowing system. In Balancer’s case this is unique in that it is the first to adopt a liquidity pool token as the mechanism for governance, the BAL/WETH 80/20 pool token.

Both quantity of the token locked, and the period of locking will determine the voting strength a holder wields. Quite simply this is defined by the number of weeks locked multiplied by the number of tokens locked itself and decays on a weekly basis. One week is considered an epoch. Voting function shown below:

![](<../../.gitbook/assets/Screen Shot 2022-04-01 at 8.26.58 PM.png>)

![](<../../.gitbook/assets/Screen Shot 2022-03-19 at 7.55.41 PM.png>)

This means that commitment to hold BAL long term will give the strength to long term holders more so than those who lock in short periods of time. Voting decay will follow a linear curve on a weekly model meaning locking for 52 weeks will give a voter 52x the voting strength than that of a holder who locks for 1 week.

The voting strength will decay over time and can accumulate if a user locks separate amounts at different points in time. Please note quantifiably, locking 1 BPT for 1 year equates to holding 1 veBAL, then the multiplier works in a fractional fashion. Locking 1 BPT for 26 weeks would yield 0.5 veBAL.

Ultimately, the benefits of the veBAL tokenomics will be felt by the BAL/WETH liquidity providers with long term commitment. Aligning governance and financial incentives to be encompassed in the token’s nature make it organically more desirable.&#x20;

In short, governance is enhanced, and the protocol revenue distributions, liquidity mining incentive boosts and the ability to direct the incentives all come to token holders in one package. This is a huge step forward to make Balancer more sustainable, while at the same time is still an upgradable system in the case that future advancements are made.
