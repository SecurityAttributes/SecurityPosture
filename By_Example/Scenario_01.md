# Security Posture by Example

## Scenario 1 - Overall Posture on the Corporate Dashboard
In this example, Amalgamated Example Company
has a very complex security posture based on
many factors across many internal organization,
located in many places.
But for the purpose of an executive dashboard,
the security posture is bucketed into one of four states:
- Business As Usual
- Heightened Threat
- Active Attack, no known material consequences foreseen
- Active Attack with material consequences

This "situational awareness status" is one measure of the
organization's security posture, and is itself a posture attribute
used in the playbooks.

One of the corporate subsidiaries (HDO.Amalgamated.Example.com) is a large
Healthcare Delivery Organization (HDO).

In Scenario 1, the status was "Business As Usual"
when the STIX object was received from the HS-ISAC.
The first step in the CACAO playbook was a decision
based on the situational awareness status.
They CACAO playbook will be oversimplified in these
scenarios but more complete CACAO use cases may be found
[here](../Use_Cases/CACAO/CacaoPaceScenario01.md).
See
[here](../Use_Cases/OpenC2/Oc2PaceScenario01.md)
for how this attribute was retrieved from the organization's
PACE system using OpenC2 commands.

Based on the organization's security policies and the
source/rating/content of the STIX object,
the playbook went down the path to change the status
from "Business As Usual" to "Heightened Threat"
until more is known on the risk of this threat.
