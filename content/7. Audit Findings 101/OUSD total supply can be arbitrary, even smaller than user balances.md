
# 41 - [OUSD total supply can be arbitrary, even smaller than user balances](./OUSD%20total%20supply%20can%20be%20arbitrary,%20even%20smaller%20than%20user%20balances.md)

The OUSD token contract allows users to opt out of rebasing effects. 

At that point, their exchange rate is “fixed”, and further rebases will not have an impact on token balances (until the user opts in).

### Recommendation:
Short term, we would advise making clear all common invariant violations for users and other stakeholders. Long term, we would recommend designing the system in such a way to preserve as many commonplace invariants as possible.
___
## Slide Screenshot
![041.png](../../images/7.%20Audit%20Findings%20101/041.png)
___
## Slide Text
- ToB Audit Origin Dollar Finding 23
- Data Validation
- High Severity
- Total Supply < Balances
- Optional Rebasing
- Specify Invariants
- Prevent Violations
___
## References
- Youtube Reference
- High Risk severity finding from [ToB’s Audit of Origin Dollar](https://github.com/trailofbits/publications/blob/master/reviews/OriginDollar.pdf)
___
## Tags
