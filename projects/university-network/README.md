# University Network Design and Access Control

## Project Overview

This project documents the design, configuration, testing, and troubleshooting of a multi-department university network implemented using Cisco Packet Tracer.

The project was developed as part of my practical networking training during SIWES and was used to apply concepts including IP addressing, subnetting, VLANs, routing, switching, and Access Control Lists (ACLs).

## Project Objectives

The main objectives were to:

- Design a structured network for multiple university departments
- Assign appropriate IP addressing schemes
- Separate departments using VLANs
- Enable communication between required networks
- Configure routing between different network segments
- Apply access-control policies to restrict specific communication paths
- Test connectivity and troubleshoot configuration problems

## Network Departments

The original design included five main departments:

| Department | VLAN |
|---|---:|
| Administration | 10 |
| ICT | 20 |
| Students | 30 |
| Library | 40 |
| Finance | 50 |

Additional VLANs and infrastructure networks were introduced during later iterations of the project as the topology was expanded.

## Technologies and Concepts Used

- Cisco Packet Tracer
- IPv4 addressing
- Subnetting
- VLANs
- Access ports
- Trunk ports
- IEEE 802.1Q
- Inter-VLAN routing
- Router configuration
- Switch configuration
- DHCP
- Access Control Lists (ACLs)
- Ping and connectivity testing
- Network troubleshooting

## Network Design

The topology was designed to represent a university environment containing multiple departments with separate logical network segments.

Each department was assigned a VLAN to provide logical separation.

A simplified representation is:

```text
                    Router / Layer 3 Device
                            |
                         Trunk
                            |
                       Core Switch
          _________________|_________________
         |          |          |          |          |
       VLAN 10    VLAN 20    VLAN 30    VLAN 40    VLAN 50
       Admin       ICT      Students     Library   Finance

The topology evolved during implementation as additional switches, servers, and routing requirements were introduced.

VLAN Configuration

VLANs were used to separate departments into different broadcast domains.

VLAN	Department
10	Administration
20	ICT
30	Students
40	Library
50	Finance

Each VLAN could then be assigned its own IP subnet and gateway.

Routing

Routing was configured to allow communication between the required VLANs and network segments.

Inter-VLAN routing allowed devices in separate VLANs to communicate through a Layer 3 device, subject to the configured access-control policies.

Access Control

Access Control Lists were introduced to control communication between departments.

The project included requirements where some departments were permitted to communicate with others while return communication was restricted.

Examples included:

Administration communicating toward ICT while restricting unwanted return traffic
Students communicating toward the Library network while restricting the reverse direction
Finance communicating toward ICT while restricting the reverse direction

These policies were implemented to demonstrate how network traffic can be selectively controlled rather than allowing unrestricted communication between all departments.

Verification and Testing

Network connectivity was tested using:

ping

Testing was performed between devices within the same network and across different VLANs.

The testing process was used to verify:

IP addressing
Default gateways
VLAN membership
Trunk connectivity
Inter-VLAN routing
ACL behavior
End-to-end connectivity
Troubleshooting

Several configuration issues were encountered during implementation.

Troubleshooting involved checking:

Physical connections
Switch port assignments
VLAN membership
Trunk configuration
IP addressing
Default gateways
Router interfaces
Routing configuration
ACL configuration

One example involved a department being connected to a switch port that had not been assigned to the correct VLAN. Correcting the port assignment restored the expected communication.

The troubleshooting process reinforced the importance of checking the network from the physical layer upward instead of assuming that a problem exists only at the routing or application layer.

Security Relevance

The project provided practical exposure to several network security principles:

Network Segmentation

VLANs were used to separate departments into distinct broadcast domains.

Access Control

ACLs were used to define which networks could communicate with each other.

Least Privilege

Communication was restricted where it was not required rather than allowing unrestricted access between departments.

Monitoring and Verification

Connectivity testing was used to confirm that implemented policies produced the expected network behavior.

Skills Demonstrated

Through this project, I practiced:

Network topology design
IPv4 addressing
Subnetting
VLAN configuration
Trunk configuration
Routing
Inter-VLAN communication
ACL configuration
Network troubleshooting
Connectivity verification
Basic network security design
Lessons Learned

One of the most important lessons from this project was that network configuration is highly interconnected.

A problem with a switch port, VLAN assignment, trunk, IP address, routing configuration, or ACL can affect communication even when the other parts of the configuration appear correct.

The project also demonstrated how networking knowledge provides a foundation for understanding network security.

Project Status

Completed

The network was configured, tested, troubleshot, and verified in Cisco Packet Tracer.

Further security controls and more advanced security projects will be added as my cybersecurity training progresses.