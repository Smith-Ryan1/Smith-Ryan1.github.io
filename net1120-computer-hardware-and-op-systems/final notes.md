🧩 OSI Model — Expanded Notes
The OSI (Open Systems Interconnection) model is a 7‑layer conceptual framework that standardizes how data moves across a network.

✅ Layers (Top → Bottom)
Application Layer

Interfaces with user applications (web browsers, email clients).

Protocols: HTTP, HTTPS, FTP, SMTP, DNS.

Presentation Layer

Translates, encrypts, compresses data.

Handles formats like JPEG, MP3, ASCII.

Session Layer

Manages sessions between devices (start, maintain, end).

Responsible for checkpoints and recovery.

Transport Layer

End‑to‑end communication; segmentation; reliability.

Protocols: TCP (reliable), UDP (fast, no guarantee).

Network Layer

Logical addressing and routing.

Protocols: IPv4, IPv6, ICMP.

Devices: Routers.

Data Link Layer

Physical addressing (MAC), error detection, frames.

Devices: Switches, bridges.

Sub‑layers: LLC, MAC.

Physical Layer

Bits on the wire; cables, connectors, voltages.

Devices: Hubs, repeaters.

🌐 TCP/IP Model — Expanded Notes
The TCP/IP model is a 4‑layer practical model used in real‑world networking.

✅ Layers (Top → Bottom)
Application Layer

Combines OSI’s Application + Presentation + Session layers.

Protocols: HTTP, DNS, DHCP, FTP, SMTP.

Transport Layer

Same as OSI Transport.

TCP = reliable, connection‑oriented.

UDP = fast, connectionless.

Internet Layer

Same as OSI Network layer.

Handles logical addressing and routing.

Protocols: IPv4, IPv6, ICMP.

Network Access Layer

Combines OSI Data Link + Physical layers.

Deals with MAC addresses, frames, bits, cabling.

🔢 IPv4 Structure — Expanded Notes
IPv4 is a 32‑bit address used to identify devices on a network.

✅ Format
Written as four decimal numbers separated by dots Example: 192.168.1.10

Each number (octet) = 8 bits Total: 32 bits → 
2
32
 possible addresses.

✅ Address Classes
Class A

Range: 1.0.0.0 – 126.255.255.255

Default mask: 255.0.0.0

Large networks.

Class B

Range: 128.0.0.0 – 191.255.255.255

Default mask: 255.255.0.0

Medium networks.

Class C

Range: 192.0.0.0 – 223.255.255.255

Default mask: 255.255.255.0

Small networks.

Class D

224.0.0.0 – 239.255.255.255

Multicast.

Class E

240.0.0.0 – 255.255.255.255

Experimental.

✅ Private IP Ranges
Class A private: 10.0.0.0 – 10.255.255.255

Class B private: 172.16.0.0 – 172.31.255.255

Class C private: 192.168.0.0 – 192.168.255.255

Used inside LANs; not routable on the internet.

✅ Subnet Masks
Subnet masks determine network vs host portions.

Examples:

255.0.0.0 → /8

255.255.0.0 → /16

255.255.255.0 → /24

CIDR notation (/24, /16, etc.) tells you how many bits belong to the network.

✅ Special IPv4 Addresses
0.0.0.0 → Default route / “any”

127.0.0.1 → Loopback

169.254.x.x → APIPA (assigned when DHCP fails)

255.255.255.255 → Broadcast
