# Security Posture by Example

## Scenario 12 - Software Development - Demming

Amalgamated Example Company has a subsidiary, EntertainMod,
that is a Tier 1 supplier to the automotive industry.
They produce
integrated entertainment modules for the large automative OEMs.
EntertainMod products
have traditionally followed Demmings principles
for hardware
and the recent surge in SBOM popularity led them
to consider doing if for software as well.
They install a PACE system and change their contract language
to require all their suppliers
to supply SBOMs directly into the PACE system thru an API.

Demming Principles:
- select the highest-quality suppliers
- select the highest-quality parts from those highest-quality suppliers
- keep track of where each part is

PACE queries (see use cases ?, ?, ?) can provide input
into historical performance of suppliers and of the
open source components used both by EntertainMod and by their suppliers.
This data can be analyzed and used to determine which are the
highest quality suppliers and which suppliers
(or components further upstream)
require more scrutiny.
