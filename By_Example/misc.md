# Security Posture by Example


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
- Software provenance and pedigree
---
