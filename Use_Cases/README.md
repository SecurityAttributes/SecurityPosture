# Use Cases

This section still under development.

See [Examples](../By_Example) for the examples that these
use cases fit into.

The use cases are organized by the standards they are
illustrating.
In other words, the use cases are a view from a specific
standard's viewpoint, are more atomic, and have more detail.

To illustrate, in the
[Scenario_01](../By_Example/Scenario_01.md)
scenario,
it is about the overall posture on the corporate dashboard.
The scenario is triggered by receiving
a STIX object from
the HS-ISAC which triggers an CACAO playbook
containing OpenC2 commands
to change the posture in a PACE system.

The need-to-fillin
STIX use case focuses on that example
from a STIX viewpoint.
It contains the details of the STIX object that initiates
the scenario.
The need-to-fillin
CACAO use case focuses on the CACAO playbook in that example.
The need-to-fillin
OpenC2 use cases focus on the actual OpenC2 commands
sent in that example.
For example the playbook has in it an OpenC2 command
to update the PACE system to change the corporate status
from "Business As Usual" to "Heightened Threat".
The need-to-fillin PACE use cases
shows those interaction from the PACE system's viewpoint.

Kestrel and SBOM were not used in that particular scenario
but their use cases will show up in other scenarios.

- [CACAO](./CACAO)
- [PACE]](./PACE)
- [OpenC2](./OpenC2)
- [Kestrel](./Kestrel)
- [SBOM](./SBOM)
