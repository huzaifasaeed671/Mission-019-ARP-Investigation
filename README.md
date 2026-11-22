# Mission 019 – ARP Investigation

## Overview
This project demonstrates practical investigation of the Address Resolution Protocol (ARP) using Wireshark and Windows PowerShell.

The objective was to capture ARP traffic, identify ARP Requests and Replies, analyze IP-to-MAC address resolution, and observe ARP cache behavior.

## Lab Environment
- Operating System: Windows
- Packet Analyzer: Wireshark
- Network Interface: Wi-Fi
- Computer IP: `192.168.1.35`
- Default Gateway: `192.168.1.1`

## Tasks Completed
- Captured ARP traffic using Wireshark.
- Identified ARP Request and ARP Reply packets.
- Examined Ethernet II and ARP packet details.
- Identified IPv4-to-MAC address mappings.
- Attempted ARP cache deletion and performed connectivity testing.
- Analyzed the final ARP packet capture.

## Key Findings

| Device | IPv4 Address | MAC Address |
|---|---|---|
| Computer | 192.168.1.35 | 4C:1D:96:95:7E:64 |
| Gateway | 192.168.1.1 | E8:43:68:2A:DC:B8 |

- ARP Request uses opcode 1.
- ARP Reply uses opcode 2.
- Packet 135 showed the computer requesting the gateway's MAC address.
- Packet 136 showed the gateway replying with its MAC address.

## Repository Structure

```text
Mission-019-ARP-Investigation/
│
├── Documentation/
│   ├── ARP-Investigation.md
│   └── ARP-Investigation.pdf
│
├── Screenshots/
│   ├── 01-Initial-ARP-Cache.png
│   ├── 02-ARP-Request-Reply.png
│   ├── 03A-ARP-Request-Details.png
│   ├── 03B-ARP-Reply-Details.png
│   └── 04-Final-ARP-Capture.png
│
└── README.md
```

## Learning Outcome
Gained practical experience analyzing ARP communication, understanding broadcast requests and direct replies, and identifying IP-to-MAC address mappings at the packet level.

**Status: Completed**
