# Security Posture by Example

## Scenario 10 - Software Development - architecture

An unexpected benefit
(although it should not have been unexpected as it occurs in most cases)
of [the previous example](./Scenario_09.md)
occurred due to discovered duplications in architecture of many products.
Simple PACE queries allowed the software developers to find
multiple copies of a given open source module,
frequently with different versions.
Reducing the duplication resulted both in reducing complexity
and in reducing the size of the executable which was particularly
important in some constrained products.
[Value Stream Mapping](add link to VSMI TC) also uncovered some
savings to be gained by consolidating support in areas with significant
commonality.
