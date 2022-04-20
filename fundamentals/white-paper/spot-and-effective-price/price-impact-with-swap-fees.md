# Price Impact - With Swap Fees

Example 4 – Including Trading Fees

To go one step further we can incorporate the trade fees into our trade. Ultimately our effective price will be altered due to the token we are selling being used to meet the swap fee. The incorporation of the pool swap fees can be done in the effective price function as follows:

![](<../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.50.50 PM.png>)

This will account for less tokens being put into the pool because they were absorbed by the fee. Therefore lower price impact is expected due to a slightly smaller trade occurring,

![](<../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.51.19 PM.png>)

Price impact now yields:

![](<../../../.gitbook/assets/Screen Shot 2022-04-01 at 7.51.49 PM.png>)
