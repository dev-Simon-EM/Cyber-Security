# Network Devices

## Overview

Network devices perform different roles in establishing, managing, and facilitating communication between systems.

During my SIWES training, I studied different categories of network devices and how they participate in network communication.

## End Devices

End devices are devices that serve as the source or destination of network communication.

Examples include:

- Desktop computers
- Laptops
- Smartphones
- Servers
- Network printers

These devices generate or receive data transmitted across a network.

## Intermediary Devices

Intermediary devices connect end devices and help control the movement of data across a network.

Examples include:

- Switches
- Routers
- Wireless access points
- Firewalls

These devices can determine where traffic should be forwarded and can provide different forms of network control.

## Hub

A hub is a basic Layer 1 networking device that repeats incoming signals to multiple connected ports.

Because a hub does not intelligently determine the intended destination of a frame, traffic is typically forwarded to all connected devices.

Hubs have largely been replaced by switches in modern Ethernet networks.

## Switch

A switch primarily operates at the Data Link layer and uses MAC addresses to make forwarding decisions.

A switch learns source MAC addresses and builds a MAC address table that helps it determine which port should receive a frame.

Switches are commonly used to connect multiple devices within a LAN.

## Router

A router operates primarily at the Network layer and uses IP addresses to determine how packets should be forwarded between different networks.

Routers can:

- Connect different networks
- Forward packets
- Provide inter-network communication
- Participate in routing protocols
- Apply access-control policies

Router configuration became an important part of the practical networking exercises during my SIWES training.

## Server

A server provides services or resources to other devices on a network.

Examples include:

- Web servers
- DNS servers
- DHCP servers
- File servers
- Application servers

During practical exercises, servers were used to provide services such as DHCP and web access within network environments.

## Network Devices in Communication

A simple communication path may involve several devices:

```text
End Device
    |
    v
Switch
    |
    v
Router
    |
    v
Destination Network
    |
    v
Server / End Device