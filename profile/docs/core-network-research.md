# Core Network Security Research

## Overview

The core network provides central functionality for mobility management, session management, authentication, and routing in telecommunication networks. This research area focuses on the security aspects of core network elements across different network generations.

## Research Areas

### Authentication and Authorization

- **Authentication Frameworks**
  - AKA (Authentication and Key Agreement)
  - EAP-AKA/EAP-AKA'
  - 5G-AKA
  - EAP-TLS implementation

- **Subscriber Identity Protection**
  - TMSI/GUTI allocation security
  - SUPI/SUCI concealment
  - IMSI/IMEI security
  - Identity request procedures

- **Authorization Mechanisms**
  - Policy enforcement
  - Subscriber profile security
  - Network slice authorization
  - Service authorization

### Signaling Security

- **SS7 Security**
  - MAP security
  - CAMEL security
  - ISUP protection
  - SS7 filtering

- **Diameter Security**
  - Command filtering
  - Application-level security
  - Transport security (SCTP/TLS)
  - AVP validation

- **HTTP/2 and SBA Security**
  - API security in 5G
  - OAuth 2.0 implementation
  - TLS profile conformance
  - Certificate management

### Core Network Elements

- **4G Core Elements**
  - MME security
  - HSS vulnerabilities
  - SGW/PGW security
  - PCRF security

- **5G Core Elements**
  - AMF security
  - UDM/AUSF/UDR security
  - SMF/UPF security
  - NRF/NSSF security considerations

- **Control Plane/User Plane**
  - CUPS security
  - N4 interface security
  - Sx interface protection
  - GTP-u security

### Interconnect and Roaming

- **Interconnect Security**
  - IPX security
  - Border gateway security
  - Interconnect firewall design
  - Traffic filtering rules

- **Roaming Security**
  - Roaming interface protection
  - SEPP (Security Edge Protection Proxy)
  - Home-routed vs. local breakout
  - Steering of roaming security

- **Network Function Security**
  - SEPP security
  - SCP (Service Communication Proxy)
  - NEF (Network Exposure Function)
  - NWDAF security

### Virtualization Security

- **NFV Security**
  - MANO security
  - VNF security requirements
  - NFV infrastructure security
  - Orchestration security

- **Container Security**
  - Kubernetes security for telco
  - Container image security
  - CNI security
  - Micro-service architecture security

- **Cloud-Native Security**
  - CI/CD pipeline security
  - DevSecOps for telco environments
  - Continuous security monitoring
  - Security policy as code

### Network Slicing Security

- **Slice Isolation**
  - Resource isolation mechanisms
  - Control plane isolation
  - User plane isolation
  - Management plane isolation

- **Slice-Specific Authentication**
  - Network slice selection
  - Slice-specific credentials
  - Multi-slice authentication
  - Slice access control

## Key Vulnerabilities

- SS7/Diameter filtering bypass
- GTP tunnel hijacking
- HSS/UDM data manipulation
- Subscriber profile modification
- Inter-PLMN security breaches
- Network slice isolation violations
- API-level attacks in 5G SBA

## Research Methodologies

- Core network penetration testing
- Signaling security assessment
- Roaming security testing
- Protocol conformance testing
- Core network fuzzing
- Virtualization security validation
- Container security assessment

## Practical Labs

1. [SS7/Diameter Security Testing](labs/01-signaling-security.md)
2. [Core Network Element Security](labs/02-core-element-security.md)
3. [Roaming Security Analysis](labs/03-roaming-security.md)
4. [Network Slicing Security](labs/04-network-slicing.md)
5. [5G Service-Based Architecture Security](labs/05-sba-security.md)

## Related Standards

- 3GPP TS 33.210: Network Domain Security
- 3GPP TS 33.310: Network Domain Security Authentication Framework
- 3GPP TS 33.501: Security architecture and procedures for 5G System
- GSMA FS.11: SS7 Interconnect Security Monitoring Guidelines
- GSMA FS.19: Diameter Interconnect Security
