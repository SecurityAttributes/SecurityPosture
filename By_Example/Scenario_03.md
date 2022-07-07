# Security Posture by Example

## Scenario 3 - Different Back to Business as Usual
This scenario has mostly the same attributes as Scenario 2
with the exception that the PACE SBOM evaluation query returned
one SBOM which does contain one affected component.

An asset management query is launched to confirm there are no
"known unknowns" (ie missing or incomplete SBOMs) in any level 1/2
devices, and there are not.
However there is one level 2 device that does contain an SBOM with
the affected component.

The playbook launches another PACE query about this SBOM to discover
if any [VEX](../GLOSSARY.md#VEX) exist for this SBOM/device.
The existence of VEX is a security posture attribute,
and the VEX contains further security posture attributes.
In this scenario, a [CSAF/VEX](../GLOSSARY.md#CSAF) does exist.
The CSAF/VEX for this device contains:
- status = NOT_AFFECTED
- status justification = vulnerable_code_not_present
The HDO security policy is to trust this particular vendor when
they say that although the component is used, the vulnerable code
has been removed.
So the HDO determines this is not a threat
the next step in the CACAO playbook
and the playboook changes the corporate situational status back to
"Business as usual".
