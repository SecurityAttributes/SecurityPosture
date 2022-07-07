# Security Posture by Example

## Scenario 4 - Heightened Threat, Automated Patch

This scenario is very similar to scenario 3.
The one difference is that the CSAF/VEX
says status = AFFECTED and recommends a patch.
Because it the device is categorized
(ie has posture attribute equal to) level 2
(ie loss/compromise may lead reduced level of care at the HDO)
and because a patch exists for the vulnerability,
the CACAO playbook takes the automated patching leg.
This schedules a brief delay before the next patient
and automatically loads the patch,
which is allowed under their security policy.
