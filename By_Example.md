# Security Posture by Example

It is sometimes easier for some people to understand concepts
by using examples.

Amalgamated Example Company is a large corporate conglomerate
with many business units in many industries.

The organization has a
[system of systems](./GLOSSARY.md#system_of_systems)
containing many devices, both virtual and physical.
The organization has many security policies,
a subset of which will be used in this example.
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
kicked off a CACAO playbook
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
calculated using risk quantification and value stream mapping.
The security policy also allows for exceptions
to this policy based on business needs.
Therefore the organization knows it has unpatched vulnerabilities due to:
- devices not yet patched within the time limit
- Documented Exceptions beyond the time limit
- Potentially devices with incomplete SBOMs so may contain the vulnerability

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

--- delete next? or move to end?
Posture attributes in this example include:
- the software on each device
   + as represented by an SBOM for that device
   + not there may be multiple SBOMs for a device
      - eg the operating system may have a separate SBOM from the application
      - eg there may be separate SBOMs for the source, from the build system, and from scanners run on the executables
- the vulnerabilities of the components on that device
   + ie the correlation of the SBOM with CVEs in the NVD
- VEX documents from the vendor and/or from 3rd-party analysis tools
- Vendor trust
- Software provenance and pedigree
- device criticality to the organization

---

The examples below will illustrate a sample of security posture attributes and their use in context.

## Scenario 1 - need better title
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

One of the corporate subsidiaries is a large
Healthcare Delivery Organization (HDO).

In Scenario 1, the status was "Business As Usual"
when the STIX object was received from the HS-ISAC.
The first step in the CACAO playbook was a decision
based on the situational awareness status.
They CACAO playbook will be oversimplified in these
scenarios but more complete CACAO use cases may be found
at {add reference link to particular CACAO use case}.
See {add reference link to particular PACE retrieval use case}
for how this status was retrieved from the organization's
PACE system.

Based on the organization's security policies and the
source/rating/content of the STIX object,
the playbook went down the path to change the status
from "Business As Usual" to "Heightened Threat"
until more is known on the risk of this threat.
(details immaterial to this explanation s),
