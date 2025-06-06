
🌐 1. Fundamentals of Networking
🧩 Key Components
Device	Role
Hub	Broadcasts data to all ports (obsolete in modern networks).
Switch	Learns MAC addresses; sends data only to the target port.
Router	Directs data between different networks (manages IP addresses).
Firewall	Inspects packets to allow/deny traffic based on rules.
VPN Concentrator	Handles secure VPN connections, especially in enterprises.

🔗 Routing vs Switching
Routing: Between networks (Layer 3).

Switching: Within a network (Layer 2).

Collision Domains: Each port on a switch is a separate collision domain.

Broadcast Domains: Each router interface separates broadcast domains.

🕸️ 2. Networking Models
Peer-to-Peer (P2P)
Decentralized, cheap, easy setup.

Suitable for file sharing, small/home networks.

Not secure or scalable.

Client-Server
Centralized, controlled access.

Used in web, email, file servers.

Higher cost but more secure and scalable.

📡 3. Network Media & Topologies
Medium	Signal Type
Copper (Ethernet)	Electrical
Fiber-optic	Light
Wireless	Radio waves

🧱 Topologies
Physical: Star (Ethernet), actual layout of cables.

Logical: Bus (Ethernet), how data travels logically.

🧮 4. IP Addressing & Binary Maths
IPv4
Format: 192.168.1.1

32-bit, dotted decimal, Big Endian

Special ranges: 0, 255, private IPs (192.168.x.x, 10.x.x.x)

IPv6
128-bit, written in hex.

Example: 1080:0000:0000:0000:0800:0000:417A

Binary Conversion
Decimal → Binary
Binary → Decimal
Example: 198 = 11000110
Learn via Cisco Binary Game

Hexadecimal
Base 16 (0–9, A–F)

Example: 200 = C8, 300 = 12C

🧱 5. Network Architecture & Infrastructure
LAN Architecture (2-tier / 3-tier)
Access Layer: End devices (e.g., laptops, printers)

Distribution Layer: Aggregates access switches

Core Layer: High-speed backbone (may be missing in 2-tier setups)

Missing Components to Look For:
Redundancy (backup links)

Security devices (IDS/IPS)

Proper labeling (uplinks, speeds)

🏢 6. Data Centres
Key Elements
Racks: Hold servers in cabinets.

UPS (Uninterruptible Power Supply): Provides battery power before generators start.

Spine-Leaf Architecture: Reduces latency and increases bandwidth.

Virtualised Components
Virtual Machines (VMs)

Virtual Network / Storage

Datacenter Switch Matrix

🧩 7. Distributed Systems
Logical Architecture
Clients send heartbeat signals every 3 seconds.

Systems use failover controllers for high availability.

Whitelisting and blacklisting to control access.

Problems to Watch For:
Single point of failure (SPOF)

Performance bottlenecks

Unclear network segmentation

💻 8. Modern Networking Practices
VLANs (Virtual LANs)
Segments network logically (e.g., HR, Finance).

Improves security and reduces broadcast traffic.

Trunking
Trunk Port: Carries multiple VLANs

Access Port: Used by a single VLAN

💰 9. Network Costs & Sustainability
CapEx vs OpEx
CapEx: Initial hardware investment.

OpEx: Ongoing costs (energy, maintenance).

Total Cost of Ownership (TCO)
Includes:

Equipment & Software

Setup & Training

Energy Use

Downtime Costs

Reducing Costs
Virtualisation

Preventative maintenance

Traffic shaping

Cloud services

🌱 10. Green Networking & Sustainability
Strategy	Description
Energy-efficient hardware	Reduces electricity usage.
Content Delivery Networks (CDNs)	Serve content from locations near users.
Compression & Caching	Reduce bandwidth and latency.
Net Zero	Balance emissions with removal.

🧪 Practical Skills
Microsoft Azure + Databricks Walkthrough:
Log in with GitHub Student Pack

Deploy a cluster

Create notebook

Execute scripts from the worksheet

[Level 5 Data Engineer Module 4 Topic 1 - Introduction to Networks for Data Engineers (1).pdf](https://github.com/user-attachments/files/20625860/Level.5.Data.Engineer.Module.4.Topic.1.-.Introduction.to.Networks.for.Data.Engineers.1.pdf)
