# Security Posture by Example

## Scenario 9 - Software Development - reduce unplanned work

One of the corporate subsidiaries of Amalgamated Example Company
is a manufacturer of control systems for electric utilities.
A major marketing advantage for this unit comes from it's
proprietary optimization software present in the product.

This software is designed in-house by a large team of software developers.
Like most software, the end-product contains software that is
10% written in house based on top of software that is 90% from third parties -
both commercial and open source.

This unit has not traditionally created SBOMs
as part of it's development process.
Based on benchmarking with it's peers, the unit decided to:
- incorporate creating SBOMs into it's standard build process
- implement a PACE system
When the log4j vulnerability was announced,
