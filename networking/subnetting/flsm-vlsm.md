# FLSM and VLSM

## Overview

Fixed Length Subnet Masking (FLSM) and Variable Length Subnet Masking (VLSM) are subnetting techniques used to divide IP networks into smaller subnets.

During my SIWES training, I studied both techniques, their procedures, differences, and practical applications in network design.

## FLSM

Fixed Length Subnet Masking divides a network into subnets of equal size.

Every subnet uses the same subnet mask and provides the same number of host addresses.

### Example

Consider:

`192.168.1.0/24`

If the network needs to be divided into four equal subnets, two host bits are borrowed.

`/24 → /26`

The resulting subnets are:

| Subnet | Network Address | Usable Hosts | Broadcast |
|---|---|---|---|
| 1 | 192.168.1.0/26 | 192.168.1.1–62 | 192.168.1.63 |
| 2 | 192.168.1.64/26 | 192.168.1.65–126 | 192.168.1.127 |
| 3 | 192.168.1.128/26 | 192.168.1.129–190 | 192.168.1.191 |
| 4 | 192.168.1.192/26 | 192.168.1.193–254 | 192.168.1.255 |

Each subnet contains 64 total addresses and traditionally 62 usable host addresses.

## VLSM

Variable Length Subnet Masking allows different subnets within the same network to use different subnet masks.

This makes it possible to allocate address space according to the actual number of hosts required by each network segment.

For example, a network may require:

- A large subnet for one department
- A medium subnet for another department
- A small subnet for a point-to-point connection

Instead of assigning the same-size subnet to all of them, VLSM allows each segment to receive an appropriate subnet size.

## FLSM vs VLSM

| Feature | FLSM | VLSM |
|---|---|---|
| Subnet size | Same | Variable |
| Subnet mask | Same for all subnets | Can differ |
| Address efficiency | Lower when requirements differ | Higher |
| Complexity | Simpler | More complex |
| Best suited for | Equal-sized networks | Networks with different host requirements |

## Practical Application

FLSM and VLSM were studied as part of IP subnetting and later applied when planning network addressing schemes.

The concepts are useful when determining how many addresses should be allocated to different departments, devices, and network segments.

## Cybersecurity Relevance

Subnetting techniques contribute to network organization and segmentation.

VLSM can help structure networks according to operational requirements, while subnetting combined with VLANs, routing, and access control can help restrict communication between different network segments.

## Key Takeaway

FLSM provides a straightforward method for creating equal-sized subnets, while VLSM provides greater flexibility and address efficiency by allowing different subnet sizes.

Understanding both techniques is important for effective network design, IP address management, and network segmentation.