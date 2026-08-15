# IP Addressing and Binary Conversion

## Overview

During my SIWES networking training, I carried out practical exercises involving IPv4 addressing and binary conversion.

The exercises focused on understanding how an IPv4 address is divided into network and host portions and how binary representation is used when analyzing addresses and subnet masks.

## IPv4 Structure

An IPv4 address contains 32 bits divided into four octets.

Example:

`192.168.10.25`

Each octet contains 8 bits:

`192` | `168` | `10` | `25`

The complete address therefore contains:

`8 + 8 + 8 + 8 = 32 bits`

## Decimal to Binary Conversion

Each decimal octet can be converted into an 8-bit binary value.

For example:

`192 = 11000000`

`168 = 10101000`

`10 = 00001010`

`25 = 00011001`

Therefore:

`192.168.10.25`

becomes:

`11000000.10101000.00001010.00011001`

## Network and Host Portions

An IPv4 address consists of:

- Network portion
- Host portion

The subnet mask determines which bits belong to the network and which bits identify hosts within that network.

For example:

`192.168.10.25/24`

uses:

`255.255.255.0`

The first 24 bits represent the network portion, while the remaining 8 bits represent the host portion.

## Address Analysis

When analyzing an IPv4 network, the following information can be determined:

- Network ID
- Subnet mask
- First usable host address
- Last usable host address
- Broadcast address
- Number of usable hosts

These calculations were later applied during subnetting exercises.

## Practical Application

IPv4 addressing and binary conversion were applied during Cisco Packet Tracer exercises and network design activities.

The knowledge was used when assigning addresses to PCs, servers, routers, and other network devices.

## Cybersecurity Relevance

Understanding IP addressing makes it easier to interpret network traffic and identify communication between systems.

It is also relevant to:

- Firewall configuration
- Access control lists
- Network segmentation
- Traffic analysis
- Incident response
- Network reconnaissance

## Key Takeaway

Binary representation provides a deeper understanding of how IPv4 addressing works. This knowledge becomes particularly important when working with subnetting, routing, network segmentation, and security controls.