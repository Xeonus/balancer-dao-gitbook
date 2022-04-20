---
description: >-
  This example shows an increase in WMATIC only which evens out the ratios of
  deposit compare to the previous Multi-token example. Notice the decrease in
  price impact as the ratio is better managed.
---

# Price Impact \[2]             WMATIC / MTA / WETH

Pool traits at the time of writing:

* _**Swap fee: 0.25%**_
* _**WMATIC: 273,763**_
* _**MTA: 1,023,625**_
* _**WETH: 66.0812**_
* _**Total BPT: 249494.507172**_\


![](https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FZjjyawYFIHU1QE6T7Y7j%2Fuploads%2FMGVxZGQOuQIrRdKvEoWG%2F4?alt=media)

The changes from the [previous example](price-impact-wmatic-mta-weth.md) will be notably base value of 10,000 WMATIC in BPT changing the calculations that follow.

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-04 at 8.04.35 PM.png>)

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-04 at 8.04.47 PM.png>)

The new Base Total BPT will change the proportional values as shown below.

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-04 at 8.05.10 PM.png>)

In this case both of our Base Values for WMATIC and WETH are greater than the proportional values for an evenly distributed despot. This means that both deposits will be taxable in terms of the swap fee.

_WMATIC_

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-04 at 8.06.27 PM.png>)

_WETH_

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-04 at 8.07.43 PM.png>)

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-04 at 8.08.00 PM.png>)

Finally, we can utilize these values to compare the invariant ratios between the initial and the after-swap fees are paid. This will determine the BPT we receive as opposed to what we would without any change in spot price.

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-04 at 8.09.20 PM.png>)

Our invariant ratio, multiplied by the initial total pool tokens, will yield the total pool tokens and therefore the amount which we will receive during our deposit. This value in comparison with our Base Case will determine our price impact.

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-04 at 8.10.24 PM.png>)

![](<../../../../../.gitbook/assets/Screen Shot 2022-04-04 at 8.10.47 PM.png>)
