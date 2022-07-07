# Security Posture by Example

It is sometimes easier for some people to understand concepts
by using examples.

Amalgamated Example Company is a large corporate conglomerate
with many business units in many industries.

The organization has a
[system of systems](./GLOSSARY.md#system_of_systems)
containing many devices, both virtual and physical.
The organization has many security policies,
a subset of which will be used in these examples.
One corporate security policy is that the organization participates
in the appropriate ISAC/ISAO's, both
sharing and receiving threat information using
[STIX](./GLOSSARY.md#stix)
over
[TAXII](./GLOSSARY.md#taxii).
The organization received a STIX object from the ISAC/ISAO
containing the Indicators of Compromise (IOCs)
for a particular campaign by a particular threat actor.
It also contained the underlying techniques
used by the threat actor including the
CVEs of the vulnerabilities being exploited.  

Reception of this STIX object
kicked off a
[CACAO](./GLOSSARY.md#CACAO)
playbook
to evaluate the risk to the organization of this particular threat.
From a parochial security posture viewpoint,
the CACAO playbook can be over simplified
to decision points and actions.
For our examples the actions will be a set of
Open Command & Control (OpenC2) commands
which we will oversimplify with some descriptive comments.
We will also oversimplify the control flow to
just the security posture attributes
used in the decision points and
the PACE OpenC2 commands
to obtain (“collect”, the “C” in PACE) and
analyze (“evaluate”, the “E” in PACE) the attributes.

The organization has finite resources
and the security policy on patching known vulnerabilities
allows varying time periods to patch
depending on the perceived risk of the vulnerability,
calculated using
[risk quantification](./GLOSSARY.md#Risk_Quantification and
[value stream mapping](./GLOSSARY.md#Value_Stream_Mapping.
The security policy also allows for exceptions
to this policy if the appropriate level of management
authorizes the exception based on business needs.
Therefore the organization knows it has unpatched vulnerabilities
due to:
- Devices not yet patched within the time limit
- Documented Exceptions beyond the time limit
- Known Unknowns ie devices with incomplete SBOMs so manual labor required to understand if the device contains the vulnerability.

The CACAO playbook kicked off above
will re-evaluate the security posture
of all the organization’s devices based on posture attributes.
Based on this re-evaluation and the organization’s security policies,
for each device the CACAO playbook will:
- do nothing
- Automatically patch
- Sandbox
- Increased monitoring
- Kick off threat hunting

The examples below will illustrate a sample of
security posture attributes and their use in context.
They make the most sense when read in order.

## Scenario 1 - Overall Posture on the Corporate Dashboard
See [Scenario 1](./Scenario_01.md)

## Scenario 2 - Back to Business as Usual
See [Scenario 2](./Scenario_02.md)

## Scenario 3 - Different Back to Business as Usual
See [Scenario 3](./Scenario_03.md)

## Scenario 4 - Heightened Threat, Automated Patch
See [Scenario 4](./Scenario_04.md)

## Scenario 5 - Heightened Threat, Increased Monitoring
See [Scenario 5](./Scenario_05.md)

## Scenario 6 - Heightened Threat, Start Threat Hunting
See [Scenario 6](./Scenario_06.md)

## Scenario 7 - Active Attack, no known material consequences foreseen
See [Scenario 7](./Scenario_07.md)

## Scenario 8 - Active Attack with material consequences
See [Scenario 8](./Scenario_08.md)

## Scenario 9 - Software Development - reduce unplanned work
See [Scenario 9](./Scenario_09.md)

## Scenario 10 - Software Development - architecture
See [Scenario 10](./Scenario_10.md)

## Scenario 11 - Software Development - license
See [Scenario 11](./Scenario_11.md)

## Scenario 12 - Software Development - Demming
See [Scenario 12](./Scenario_12.md)

## Scenario 13 - Software Development - predictive
See [Scenario 13](./Scenario_13.md)

## Scenario 14 - Build systems
See [Scenario 14](./Scenario_14.md)

## Scenario 15 - Software provenance and pedigree
See [Scenario 15](./Scenario_15.md)

## Scenario 16 - Software provenance and pedigree
See [Scenario 16](./Scenario_16.md)

## Scenario 17 - Vendor trust
See [Scenario 17](./Scenario_17.md)

## Scenario 18 - M&A
See [Scenario 18](./Scenario_18.md)
