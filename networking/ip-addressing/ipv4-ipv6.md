# IPv4 and IPv6 Addressing

## Overview

IP addressing provides logical identification for devices communicating across a network.

During my SIWES training, I studied IPv4 and IPv6 addressing, their structures, differences, and practical applications in computer networking.

## IPv4

IPv4 uses a 32-bit address divided into four 8-bit octets.

An IPv4 address is normally written in dotted-decimal notation.

Example:

`192.168.1.10`

Each octet can have a value from 0 to 255.

The same address in binary is:

`11000000.10101000.00000001.00001010`

## IPv4 Address Classes

Traditional IPv4 addressing divides addresses into five classes:

| Class | First Octet Range | General Use |
|---|---:|---|
| A | 1–126 | Large networks |
| B | 128–191 | Medium-sized networks |
| C | 192–223 | Smaller networks |
| D | 224–239 | Multicast |
| E | 240–255 | Experimental/reserved |

The address `127.0.0.0/8` is reserved for loopback and is therefore not part of the normal Class A host range.

## Private IPv4 Address Ranges

Private IPv4 addresses are commonly used inside local networks.

| Range | CIDR |
|---|---|
| 10.0.0.0 – 10.255.255.255 | 10.0.0.0/8 |
| 172.16.0.0 – 172.31.255.255 | 172.16.0.0/12 |
| 192.168.0.0 – 192.168.255.255 | 192.168.0.0/16 |

These addresses are commonly used for internal networks and are not directly routable across the public Internet.

## IPv6

IPv6 uses 128-bit addresses and was developed to provide a much larger address space than IPv4.

An IPv6 address is represented using hexadecimal notation.

Example:

`2001:db8:abcd:0012:0000:0000:0000:0001`

IPv6 addresses can be shortened using zero-compression rules.

For example:

`2001:db8:abcd:12::1`

## IPv4 vs IPv6

| Feature | IPv4 | IPv6 |
|---|---|---|
| Address size | 32 bits | 128 bits |
| Representation | Decimal | Hexadecimal |
| Address space | Smaller | Extremely large |
| Example | 192.168.1.10 | 2001:db8::1 |
| Broadcast | Supported | No traditional broadcast |
| Address configuration | Manual/DHCP | SLAAC, DHCPv6, manual |

## Binary Conversion

Understanding binary representation was an important part of the IPv4 addressing exercises.

For example:

`192.168.1.10`

can be represented as:

`11000000.10101000.00000001.00001010`

Converting between decimal and binary makes it easier to understand subnet masks, network boundaries, host ranges, and subnetting.

## Cybersecurity Relevance

IP addressing is important in cybersecurity because IP addresses are used to identify network endpoints and analyze communication.

Understanding IPv4 and IPv6 helps with:

- Network traffic analysis
- Firewall rules
- Access control
- Network monitoring
- Incident investigation
- Network reconnaissance
- Identifying source and destination hosts

## Practical Application

The concepts were applied during networking exercises using Cisco Packet Tracer, where IP addresses were assigned to devices and used for communication between hosts, switches, routers, and servers.

## Key Takeaway

Understanding IP addressing provides the foundation for subnetting, routing, network configuration, traffic analysis, and many network security activities.