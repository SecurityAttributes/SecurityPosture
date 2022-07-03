# Security Posture by Example

Amalgamated Example is a large corporate conglomerate
with many business units in many industries.
The organization has a system of systems
containing many devices, both virtual and physical.
The organization has many security policies,
a subset of which will be used in this example.
One corporate security policy is that the organization participates
in the appropriate ISAC/ISAO, both
sharing and receiving threat information using STIX over TAXII.
The organization received a STIX object from the ISAC/ISAO
containing the Indicators of Compromise (IOCs)
for a particular campaign by a particular threat actor.
It also contained the underlying techniques
used by the threat actor including the
CVEs of the vulnerabilities being exploited.  
Reception of this STIX object
kicked off a CACAO playbook
to evaluate the risk to the organization of this particular threat.
 The organization has finite resources
 and the security policy on patching known vulnerabilities
 allows varying time periods to patch
 depending on the perceived risk of the vulnerability,
 calculated using risk quantification and value stream mapping.
The security policy also allows for exceptions
to this policy based on business needs.
Therefore the organization knows it has unpatched vulnerabilities due to:
- devices not yet patched within the time limit
- Documented Exceptions beyond the time limit
- Potentially devices with incomplete SBOMs so may contain the vulnerability

The CACAO playbook kicked off above
will re-evaluate the security posture
of all the organization’s devices based on posture attributes.
Based on this re-evaluation and the organization’s security policies,
for each device the CACAO playbook will:
- do nothing
- Automatically patch
- Sandbox
- Increased monitoring
- Kick off threat hunting

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
