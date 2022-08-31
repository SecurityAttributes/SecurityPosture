# Security Posture by Example

## Scenario 20 - Heightened Threat, Known Unknowns

This scenario is for the HDO in
[Scenario 2](./Scenario_02.md)
but is different because in this case
there is a CSAF/VEX for that CVE
for at last one vendor.
The status is AFFECTED
and there are known exploits in the wild.
The HDO can patch the known vendor product but
unfortunately the HDO does not have complete SBOMs
for many other products from other vendors.

In this situation, the HDO must a manual
effort to call vendors, use 3rd-party scanning tools,
and assess device by device whether the devices may be affected
and what to do about it.
Because of the risk, they start threat hunting with
[Kestrel](../GLOSSARY.md#kestrel).
