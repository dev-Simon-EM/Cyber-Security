# Unicast, Multicast, and Broadcast Communication

## Overview

Network communication can be classified according to the number of intended receivers.

During my SIWES training, I studied three common transmission methods:

- Unicast
- Multicast
- Broadcast

Understanding these communication patterns is important for network operation and traffic analysis.

## Unicast

Unicast is a one-to-one communication method.

A sender transmits data to one specific destination.

```text
Device A ───────→ Device B
           ┌──→ Device B
Device A ──┼──→ Device C
           └──→ Device D
           ┌──→ Device B
           ├──→ Device C
Device A ──┼──→ Device D
           └──→ Device E
