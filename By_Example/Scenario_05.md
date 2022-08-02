# Security Posture by Example

## Scenario 5 - Heightened Threat, Increased Monitoring
This scenario is similar to Scenario 3 except the CSAF/VEX comes back
with
- status = NOT_AFFECTED
- status justification = vulnerable_code_cannot_be_controlled_by_adversary.

Although the HMO does trust that the vendor
used the correct status justification,
the HDO security policy is to increase monitoring in this situation.
So the CACAO playbook increases monitoring on the device with the
potentially vulnerable component.

Here is the policy as implemented in CACAO
![policy](./IIID01.png).
See
[here](../Use_Cases/CACAO/CacaoPaceScenario05.md)
for the actual CACAO playbook.
See
[here](../Use_Cases/OpenC2/Oc2PaceScenario05.md)
for interfacing with the
PACE system using OpenC2 commands.
