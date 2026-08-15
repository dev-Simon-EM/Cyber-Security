# Ethernet Frame and LAN Communication

## Overview

Ethernet is a widely used technology for communication within local area networks (LANs). It operates primarily at the Physical and Data Link layers of the OSI model.

During my SIWES training, I studied the Ethernet frame structure, the purpose of its fields, and how Ethernet supports communication between devices on a LAN.

## Ethernet Frame Structure

An Ethernet frame contains several fields used to deliver and process data across a local network.

The main fields include:

| Field | Purpose |
|---|---|
| Preamble | Helps synchronize communication between sender and receiver |
| Start Frame Delimiter (SFD) | Indicates the beginning of the frame |
| Destination MAC Address | Identifies the intended receiving device |
| Source MAC Address | Identifies the device that transmitted the frame |
| Type/Length | Identifies the upper-layer protocol or the length of the payload |
| Data and Padding | Carries the encapsulated data and may include padding when necessary |
| Frame Check Sequence (FCS) | Used for error detection |

## Ethernet Frame Length

A standard Ethernet frame has:

- Minimum size: **64 bytes**
- Maximum standard size: **1518 bytes**, excluding the preamble and SFD

The frame size requirements help ensure reliable operation of Ethernet networks.

## MAC Addresses

Ethernet uses Media Access Control (MAC) addresses to identify network interfaces at the Data Link layer.

A MAC address is typically represented as six hexadecimal octets.

Example:

`00:1A:2B:3C:4D:5E`

The destination MAC address identifies where the frame should be delivered on the local network, while the source MAC address identifies the sender.

## Ethernet and Encapsulation

When data moves down the networking stack, information from higher layers is encapsulated into an Ethernet frame at the Data Link layer.

A simplified process is:

```text
Application Data
      ↓
Transport Segment
      ↓
IP Packet
      ↓
Ethernet Frame
      ↓
Bits on the Physical Medium