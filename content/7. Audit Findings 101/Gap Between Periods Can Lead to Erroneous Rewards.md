
# 75 - [Gap Between Periods Can Lead to Erroneous Rewards](./Gap%20Between%20Periods%20Can%20Lead%20to%20Erroneous%20Rewards.md)

The SNX rewards are earned each period based on reward and duration as specified in the `notifyRewardAmount()` function. 

The contract will output more rewards than it receives. 

Therefore if all stakers call `getReward()` the contract will not have enough SNX balance to transfer out all the rewards and some stakers may not receive any rewards.

### Recommendation:
We recommend enforcing each period start exactly at the end of the previous period.
___
## Slide Screenshot
![075.png](../../images/7.%20Audit%20Findings%20101/075.png)
___
## Slide Text
- Sigma Prime Unipool Finding 4
- Timing/DoS
- Medium Severity
- Stakers -> getReward()
- SNX Deficit -> No Rewards
- No Gap Between Periods
___
## References
- Youtube Reference
- Medium Risk severity finding from [Sigma Prime's Audit of Synthetix Unipool](https://github.com/sigp/public-audits/blob/master/synthetix/unipool/review.pdf)
___
## Tags
