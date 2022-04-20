---
description: >-
  In-Given-Price-Proof - Please note the prerequisites of the spot price
  function and In-Given-Out Equations.
---

# In-Given-Price Proof

In-Given-Price Proof:

1. Firstly, we must site the spot price function:

$$
SP_{i}^{o}={\frac {\frac {B_{i}}{W_{i}}}{\frac {B_{o}}{W_{o}}}}
$$

2\. Secondly, to consider the desired spot price (SP’) we must acknowledge that the Balance-In (Bi) and the Balance-Out (Bo) will be altered based on the Amount-In (Ai) and Amount-Out (Ao) as so:&#x20;

$$
SP_{i}^{'o}={\frac {\frac {B_{i}+A_{i}}{W_{i}}}{\frac {B_{o}-A_{o}}{W_{o}}}}
$$

3\. The original spot price can be rearranged to isolate the Balance-Out (Bo):

![](<../../../../.gitbook/assets/Screen Shot 2022-04-01 at 8.02.43 PM.png>)

4\. The adjusted spot price equation (SP’) can be arranged to isolate Balance-Out minus the Amount-Out (Bo – Ao) as follows:

![](<../../../../.gitbook/assets/Screen Shot 2022-04-01 at 8.03.09 PM.png>)

5\. . Using these equations for substitution in our In-Given-Out equation below we can prove the In-Given-Price Equation is valid:

$$
A_{i} = B_{i} \ * \ \Bigg(\bigg({\frac {B_{o}}{B_{o}-A_{o}}}\bigg)^{{\frac {W_{o}}{W_{i}}}}-1\Bigg)
$$

First, we replace the Balance-Out and Balance-Out minus Amount-Out statements with our equations from steps 3 and 4.

![](<../../../../.gitbook/assets/Screen Shot 2022-04-01 at 8.03.33 PM.png>)

At this point the Weights-In and Weights-Out will neutralize one another reducing our equation size, once this is done the next step is to rationalize our fraction:

![](<../../../../.gitbook/assets/Screen Shot 2022-04-01 at 8.04.01 PM.png>)

Now we need to isolate the spot price ratio to remove the Balance-In (Bi) and Amount-In (Ai) from our inner function:

![](<../../../../.gitbook/assets/Screen Shot 2022-04-01 at 8.04.57 PM.png>)

We will move our exponent to the opposite side of the equation and then adjust our ratio of Balance-In over Balance-In minus Amount-In

![](<../../../../.gitbook/assets/Screen Shot 2022-04-01 at 8.05.24 PM.png>)

Now using this adjusted ratio, we can multiply both sides of the equation by Amount-In, Balance-In portion combining the two terms and have the fraction of SP’ and SP on the right side of our equation as shown below:

![](<../../../../.gitbook/assets/Screen Shot 2022-04-01 at 8.05.52 PM.png>)

By adjusting the exponents and reverting the bulk of our equation to the right side again we can solve for the Amount-In as intended for the In-Given-Price Equation:

![](<../../../../.gitbook/assets/Screen Shot 2022-04-01 at 8.06.21 PM.png>)
