# Security Posture by Example

## Scenario 2 - Back to Business as Usual
Scenario 2 starts where Scenario 1 left off -
i.e. corporate situational level is "Heightened Threat"
and the organization has received new threat information
from the HS-ISAC in the form of a STIX object.

In this particular scenario,
the information received contains the
[CVE](../GLOSSARY.md#CVE) being exploited in the campaign,
and the HDO has a [PACE](../GLOSSARY.md#pace) system for
collecting and evaluating posture attributes.

The HDO has a security policy to categorize each of it's devices
according to the device impact on patient care
and/or financial operations::
- level 1 - loss/compromise leads to likely loss of life
- level 2 - loss/compromise may lead reduced level of care
- level 3 - loss/compromise may lead to financial impact on business
- level 4 - loss/compromise for 1 day would not greatly impact patient care or financial operations
This 'impact' attribute is both a security-
and a safety-posture attribute
which the HDO uses in it's security policies to drive certain actions
in the playbooks.
This attribute is stored in the HDO's Asset Management system.

In this scenario,
the HDO has a complete and accurate inventory of
all it's level 1 and level 2
[physical](../GLOSSARY.md#physical_device) and
[virtual](../GLOSSARY.md#virtual_device) devices.
In this scenario, it is also true that
[SBOMs](../GLOSSARY.md#sbom) have already been collected in
the PACE system for all level 1/2 devices.
These SBOMs are also posture attributes of the devices.

The HDO security policy only calls for being in the corporate
"Heightened Threat" state if there is the possibility of
loss/compromise of Level 1 or Level 2 devices.
In the previous scenario, "Heightened Threat" was raised because it
is not yet known if this threat will affect Level 1/2 devices.

A CACAO playbook is kicked off to evaluate which, if any,
devices have the vulnerable component.
A PACE evaluation query is launched
{put in link to detailed use case for this}
asking what SBOMs in the PACE system contain the vulnerable component.
The response is the null set.
An asset management query is launched to confirm there are no
"known unknowns" (ie missing or incomplete SBOMs) in any level 1/2
devices.
This query also returns the null set.

Based on this information, the next step in the CACAO playbook
is to change the corporate situational status back to
"Business as usual".

Note that the vast majority of CVE's will follow this scenario.
CVE's are created at a rate of
{need number and reference}
and the vast majority are not applicable for any given organization.
Therefore automating this scenario
should result in significant cost savings.
