# 104 - [ERC20 decimals returns a uint8](ERC20%20decimals%20returns%20a%20uint8.md)

Several tokens incorrectly return a uint256. If this is the case, ensure the value returned is below 255. (See [here](https://github.com/crytic/building-secure-contracts/blob/master/development-guidelines/token_integration.md#erc-conformity))

___
## Slide Screenshot
![0104.png](../../images/5.%20Pitfalls%20and%20Best%20Practices%20201/104.png)
___
## Slide Text
- ERC20 decimals
- Decimals in Tokne Typically 18
- Return uint8
- uint256 -> Incorrect
- Return uint256 -> Check Value <= 255
___
## References
- [Youtube Reference](https://youtu.be/WGM1SF8twmw?t=206)
___
## Tags