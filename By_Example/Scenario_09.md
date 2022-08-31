# Security Posture by Example

## Scenario 9 - Software Development - reduce unplanned work

One of the corporate subsidiaries of Amalgamated Example Company
is a manufacturer of control systems for electric utilities
NoShock.Amalgamated.Example.com.
A major marketing advantage for this unit comes from it's
proprietary optimization software present in the product.

This software is designed in-house by a large team of software developers.
Like most software, the end-product contains software that is
10% written in house based on top of software that is 90% from third parties -
both commercial and open source.

Historically, the team did not devote much time to updating
open source or commercial 3rd-party products
and instead focused on new features.
However, in recent years
a large influx of ransomware and cyber attacks
against their customers
caused business unit to slip release dates
and miss corporate financial targets
due to unplanned, unscheduled work associated
with fixing vulnerabilities in their products being exploited
by hackers.

This unit has not traditionally created SBOMs
as part of it's development process.
Based on benchmarking with it's peers,
quantitative risk analysis was performed and
the unit decided to:
- incorporate creating SBOMs into it's standard build process
- implement a PACE system

The PACE system allowed the development team
to use [Value Stream Mapping](add link to VSMI TC)
and quantitative risk analysis to allocate
the optimum level of effort to updating
open source or commercial 3rd-party products,
keeping their products secure and drastically reducing
their customers being exploited.

This reduction in unplanned, unscheduled work
got the business unit back on-schedule and meetings it's financial targets.

An additional benefit occurred
when the log4j vulnerability was announced.
Log4j caused a huge burst of unplanned, unscheduled work
throughout many companies in many industries.
Simple PACE queries (see usecases ?, ? ?)
allowed the product teams to quickly determine the products
that were and were not affected.
For the unaffected products, which was the vast majority,
VEXs were issued (created quickly using PACE, see use case ?).
The development was able to quickly focus on the few affected products,
and get patches out quickly.
Although log4j did cause unplanned, unschedule work,
the impact on Amalgamated was orders of magnitude less than it would have
been before the PACE system was implemented.
