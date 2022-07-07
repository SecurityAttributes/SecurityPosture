# Security Posture by Example

## Scenario 6 - Heightened Threat, Start Threat Hunting

This scenario is most similar to Scenario 5
except the CSAF/VEX comes back
with status = NOT_AFFECTED and status justification =
vulnerable_code_not_in_execute_path.

Although the HMO does trust that the vendor
used the correct status justification,
the HDO security policy
in this situation,
is to start threat hunting with
[Kestrel](../GLOSSARY.md#kestrel).
The HDO has been attacked too many times with chained attacks
to ignore the potential in this situation.
So the CACAO playbook starts Kestrel threathunting on the device with the
potentially vulnerable component.

Here is the policy as implemented in CACAO
![policy](./IIID01.png).
See
{add link to actual CACAO playbook in use case section}
for the actual CACAO playbook.
See
{add link to actual PACE usecases in use case section}.
See
{add link to actual OpenC2 usecases in use case section}.
See
{add link to actual Kestrel usecases in use case section}.
