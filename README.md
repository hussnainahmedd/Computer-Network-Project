<div align="center">

# 🌐 Computer Network Project

### _Enterprise network simulation for AIR University, built in Cisco Packet Tracer._

![Cisco Packet Tracer](https://img.shields.io/badge/Cisco-Packet%20Tracer-0078D4?style=for-the-badge)
![Networking](https://img.shields.io/badge/Networks-VLANs%20%7C%20Routing%20%7C%20ACLs-6C757D?style=for-the-badge)
![Academic](https://img.shields.io/badge/Academic-Coursework-6A5ACD?style=for-the-badge)

<img src="assets/hero.webp" alt="Enterprise network topology banner" width="850"/>

A complete enterprise network simulation for a university campus —
**main campus + branch campus** connected over a WAN, with department-level
VLAN segmentation, inter-VLAN routing, core services (DNS, DHCP, HTTP, FTP,
Email) and ACL-based security — designed, configured, and tested in
**Cisco Packet Tracer**.

</div>

---

## 🏛️ What this project covers

The simulation models a full university network built in one Packet Tracer file (`Project.pkt`):

- **Main campus (3 buildings)** — 8 departments, each on its own VLAN (VLAN 10–80, `192.168.1.0/24`–`192.168.8.0/24`)
- **Branch campus** — Staff (VLAN 90) and Student Lab (VLAN 100), linked to the main campus over a WAN
- **Inter-VLAN routing** — Layer 3 switching via Cisco 3650-24PS switches
- **Services** — DNS, DHCP, a university web portal, internal email, and an FTP server for the IT department
- **Security** — extended ACLs restricting each department to its own printer while keeping web/email/DNS open
- **Cloud connectivity** — external email server reachable via a cloud router

📸 The full designed topology is captured in [`topology.png`](topology.png).

---

## 🧠 Concepts applied

| Area | What was used |
|---|---|
| VLANs & Trunking | 802.1Q trunking across 10 VLANs |
| Routing | Inter-VLAN routing on L3 switches, inter-campus routing on Cisco 2911 routers |
| Services | DHCP, DNS, HTTP, FTP, SMTP/POP3 |
| Security | Extended ACLs for printer access control |
| Design | Subnet planning & address allocation |

## 🛠️ Tech stack

- **Cisco Packet Tracer** — simulation & design environment
- **Cisco 2911** routers · **3650-24PS** L3 switches · **2960-24TT** access switches
- **Server-PT** — web/DNS, FTP/DNS, and email services

## 🚀 How to run

1. Install **Cisco Packet Tracer** (free for Networking Academy members).
2. Clone this repo:
   ```bash
   git clone https://github.com/hussnainahmedd/Computer-Network-Project.git
   ```
3. Open **`Project.pkt`** in Packet Tracer.
4. Explore the topology, inspect device configs (CLI tabs), and test connectivity between VLANs and campuses.

---

<div align="center">

_Built with Packet Tracer by [Hussnain Ahmad](https://github.com/hussnainahmedd) — BSCS @ Air University, Islamabad 🇵🇰_

</div>
