# OSI and TCP/IP Models

## Overview

The OSI and TCP/IP models provide structured ways of understanding how data is transmitted between devices across a network.

During my SIWES training, I studied both models and their respective layers, functions, and roles in network communication.

## OSI Model

The Open Systems Interconnection (OSI) model consists of seven layers:

| Layer | Name | Main Function |
|---|---|---|
| 7 | Application | Provides network services to applications |
| 6 | Presentation | Handles data formatting, translation, encryption, and compression |
| 5 | Session | Establishes, manages, and terminates communication sessions |
| 4 | Transport | Provides end-to-end communication and reliability |
| 3 | Network | Handles logical addressing and routing |
| 2 | Data Link | Handles MAC addressing and frame transmission |
| 1 | Physical | Transmits raw bits through physical media |

## TCP/IP Model

The TCP/IP model is commonly represented using four layers:

| Layer | Main Function |
|---|---|
| Application | Provides network services and application-level communication |
| Transport | Provides end-to-end communication using protocols such as TCP and UDP |
| Internet | Handles logical addressing and routing using IP |
| Network Access | Handles physical transmission and local network communication |

## OSI vs TCP/IP

The OSI model provides a more detailed conceptual framework with seven layers, while the TCP/IP model groups related functions into four broader layers.

The OSI model is useful for understanding and troubleshooting networking concepts, while the TCP/IP model closely represents the protocol architecture used by modern networks.

## Cybersecurity Relevance

Understanding the networking layers is important in cybersecurity because attacks and security controls can operate at different layers.

Examples include:

- Physical security at the Physical layer
- MAC-based controls at the Data Link layer
- IP filtering and routing controls at the Network layer
- Port and connection controls at the Transport layer
- Application security controls at the Application layer

Understanding the layers also helps security professionals analyze network traffic and determine where a communication problem or security event may be occurring.

## Practical Application

The OSI and TCP/IP concepts were applied during Cisco Packet Tracer exercises involving:

- Device-to-device communication
- Switches and routers
- IP addressing
- DHCP
- Ethernet communication
- Routing
- Access control

## Key Takeaway

The OSI and TCP/IP models provide a framework for understanding how network communication occurs.

For cybersecurity, this knowledge is important because effective network defense requires understanding how devices communicate, where traffic flows, and where security controls can be applied.