# Security Posture by Example

## Scenario 14 - Build systems

Amalgamated Security is a subsidiary of
the Amalgamated Example Company
which produces and sells cybersecurity products.

Amalgamated Security recognized that what happened to Solar Winds
could also happen to Amalgamated Security because attackers
consider cybersecurity systems as high-value targets.

Amalgamated Security installs a PACE system and implements processes
to not only track the SBOMs of all the products they are producing,
but also of the tooling used
to build, install, and maintain their products.
In addition, they implement tracking all 4 types of SBOMs:
- SBOMs of the source code (source SBOMs) - see use cases ?,??
- SBOMs created by the build process (build SBOMs) - see use cases ?,??
- SBOMs created as part of the software installation process (install SBOMs) - see use cases ?,??
- SBOMs created by 3rd-party tools doing analysis on the executables (binary analysis SBOMs)  - see use cases ?,??

Amalgamated PACE system consists of both open-source
and modules from several commercial vendors.
One of the commercial Posture Evaluation System (PES) modules
is capable of analyzing SBOMs across the 4 types looking for
discrepancies and anomolies which may be indicative of
intruders attempting a Solar Winds-like attack.
