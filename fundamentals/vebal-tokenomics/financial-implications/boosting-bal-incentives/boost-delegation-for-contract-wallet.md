---
description: >-
  How to delegate boost from locking veBAL on a standard EOA to a Gnosis Safe or
  similar contract wallet / mechanism.
---

# Boost Delegation for Contract Wallet

A common obstacle faced by users of vote escrowed systems is the inability to lock their token in the time based veBAL contract. For safe users this would mean no access to veBAL governance or boosted liquidity pool incentives.&#x20;

If you would like to delegate your veBAL boost to another address, you can do so by calling the create\_boost function on the veBAL veboost contract [https://etherscan.io/address/0x2E96068b3D5B5BAE3D7515da4A1D2E52d08A2647#writeContract](https://etherscan.io/address/0x2E96068b3D5B5BAE3D7515da4A1D2E52d08A2647#writeContract)

```
// code
_delegator = your address which has veBAL,
_receiver = your address you want to boost
_percentage = 5000 // 50% (10000 is 100% of your boost)
_cancel_time = 0 // allow yourself to cancel anytime
_expire_time = 1651363200 // unix timestamp for 1st 
of may (Check this! Also your lock needs to last past this time)
_id = 0,
```

This is useful for situations where you are LP'ing from a contract like a gnosis safe which, because it's a contract, is incapable of locking of veBAL. Instead, you lock up veBAL from an EOA and delegate your boost to your gnosis safe.

Note that the percentage is flexible over the complete range of boost which you would like to delegate.

[Vyper\_contract | Address 0x2E96068b3D5B5BAE3D7515da4A1D2E52d08A2647...](https://etherscan.io/address/0x2E96068b3D5B5BAE3D7515da4A1D2E52d08A2647)
