# Routing and Switching Fundamentals

## Overview

Routing and switching are core networking functions used to move data between devices within a network and between different networks.

During my SIWES training, I studied routing and switching concepts and applied them through practical Cisco Packet Tracer exercises and network configuration projects.

## Switching

Switching is primarily used to connect devices within a local area network (LAN).

A network switch learns the MAC addresses of connected devices and uses this information to determine where Ethernet frames should be forwarded.

### MAC Address Learning

When a frame enters a switch, the switch can learn the source MAC address and associate it with the port through which the frame arrived.

The switch stores these associations in its MAC address table.

A simplified process is:

```text
Frame arrives
     |
     v
Learn source MAC
     |
     v
Check destination MAC
     |
     v
Forward or flood frame

Routing

Routing is the process of forwarding IP packets between different networks.

Routers use routing information to determine the appropriate path toward a destination network.

A simplified routing process is:

Source Network
      |
      v
   Router
      |
      v
Routing Decision
      |
      v
Destination Network
Router-to-Router Communication

During practical exercises, I configured communication between routers using Cisco IOS command-line configuration.

This involved:

Configuring router interfaces
Assigning IP addresses
Configuring appropriate network connections
Verifying interface status
Testing connectivity using ping
Troubleshooting incorrect configurations

Successful router-to-router communication demonstrates that the connected networks can exchange IP traffic through the configured path.

VLANs

A Virtual Local Area Network (VLAN) allows devices connected to the same physical switching infrastructure to be separated into logical networks.

VLANs can be used to:

Organize departments
Separate broadcast domains
Improve network management
Support network segmentation
Apply different access-control policies

For example, a university network could use separate VLANs for:

Administration
ICT
Students
Library
Finance
Access Ports

An access port is normally assigned to a single VLAN and is commonly used to connect end devices such as PCs and printers.

For example:

PC
 |
 v
Switch Access Port
 |
 v
VLAN
Trunk Ports

A trunk port carries traffic belonging to multiple VLANs across a single physical link.

IEEE 802.1Q tagging can be used to identify the VLAN associated with a frame as it crosses a trunk.

A simplified topology is:

VLAN 10 ----\
VLAN 20 ----- Switch ===== Trunk ===== Switch
VLAN 30 ----/
Inter-VLAN Routing

Devices in different VLANs cannot communicate directly through Layer 2 switching alone.

Inter-VLAN routing provides communication between different VLANs through a Layer 3 device such as a router or Layer 3 switch.

This can be implemented using:

Router subinterfaces
A Layer 3 switch with switched virtual interfaces (SVIs)
Practical Application

Routing and switching concepts were applied during Cisco Packet Tracer exercises involving:

Switch configuration
VLAN configuration
Trunk links
Router configuration
Inter-VLAN communication
Router-to-router communication
DHCP
Access control lists
Connectivity testing
Network troubleshooting
Troubleshooting

Practical networking exercises demonstrated that successful communication depends on several components being correctly configured.

Common areas checked during troubleshooting included:

Physical connections
Interface status
IP addressing
Subnet masks
Default gateways
VLAN assignments
Trunk configuration
Routing
Access-control policies

Verification tools such as ping, interface-status commands, routing information, and MAC address tables were useful for identifying configuration problems.

Cybersecurity Relevance

Routing and switching form an important foundation for network security.

VLANs can provide logical segmentation, while routing and access-control policies can determine which networks are allowed to communicate.

Understanding these mechanisms is essential when designing security controls such as:

Network segmentation
Access control
Traffic filtering
Security zones
Network monitoring
Key Takeaway

Routing determines how traffic moves between networks, while switching manages communication within local networks.

Understanding both is essential for configuring, troubleshooting, segmenting, and securing modern networks.