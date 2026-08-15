# IP Subnetting Fundamentals

## Overview

IP subnetting is the process of dividing a larger IP network into smaller logical networks called subnets.

During my SIWES training, I studied subnetting as part of the foundation required for network design, addressing, routing, and network security.

## Purpose of Subnetting

Subnetting can be used to:

- Divide a network into smaller networks
- Organize devices into logical network segments
- Reduce unnecessary broadcast traffic
- Improve IP address utilization
- Support network organization and scalability
- Provide a foundation for network segmentation and access control

## Key Subnetting Concepts

When analyzing a subnet, several important values can be determined:

- Network ID
- Subnet mask
- First usable host address
- Last usable host address
- Broadcast address
- Number of usable hosts

## Network ID

The Network ID identifies the subnet itself.

For example, for:

`192.168.1.0/24`

the Network ID is:

`192.168.1.0`

## Broadcast Address

The broadcast address is used to communicate with all hosts within a subnet.

For:

`192.168.1.0/24`

the broadcast address is:

`192.168.1.255`

## Usable Host Range

For a traditional `/24` network:

- Network address: `192.168.1.0`
- First usable host: `192.168.1.1`
- Last usable host: `192.168.1.254`
- Broadcast address: `192.168.1.255`

This provides 254 traditionally usable host addresses.

## Subnet Masks

A subnet mask identifies which portion of an IPv4 address represents the network and which portion represents hosts.

For example:

`/24 = 255.255.255.0`

The `/24` notation means that 24 of the 32 IPv4 bits are used for the network portion.

## Borrowing Host Bits

Subnetting involves borrowing bits from the host portion of an IPv4 address and using them to create additional network bits.

For example, changing a `/24` network to `/26` borrows two host bits.

This creates:

`2² = 4`

subnets.

Each `/26` subnet contains:

`2⁶ = 64`

total addresses.

Traditionally, 62 of these are usable host addresses because the network and broadcast addresses are reserved.

## Example

Consider:

`192.168.1.0/24`

Dividing it into four equal subnets requires borrowing two host bits, resulting in `/26`.

The four subnets are:

| Subnet | Network Address | Usable Host Range | Broadcast |
|---|---|---|---|
| 1 | 192.168.1.0/26 | 192.168.1.1–62 | 192.168.1.63 |
| 2 | 192.168.1.64/26 | 192.168.1.65–126 | 192.168.1.127 |
| 3 | 192.168.1.128/26 | 192.168.1.129–190 | 192.168.1.191 |
| 4 | 192.168.1.192/26 | 192.168.1.193–254 | 192.168.1.255 |

## Subnetting and Network Design

Subnetting became particularly useful during later practical network design exercises.

Different departments or network segments can be assigned different subnets, allowing administrators to organize devices and apply appropriate routing and access-control policies.

## Cybersecurity Relevance

Subnetting is also relevant to cybersecurity because logical network segmentation can help limit communication between systems.

When combined with technologies such as VLANs, routing policies, and access control lists, subnetting can contribute to:

- Network segmentation
- Access control
- Broadcast-domain separation
- Traffic management
- Limiting unnecessary network exposure

## Key Takeaway

Subnetting provides a structured method for dividing IP networks into smaller networks.

Understanding Network IDs, subnet masks, host ranges, broadcast addresses, and usable host counts is essential for designing, configuring, troubleshooting, and securing computer networks.