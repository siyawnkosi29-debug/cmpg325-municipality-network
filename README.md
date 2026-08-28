# cmpg325-municipality-network
# CMPG 325 - Computer Networks Project

 Project Overview
- **Client**: JB Marks Local Municipality Satellite Office (Ventersdorp)
- **Client ID**: CLI-105
- **Project ID**: CMPG325-2026-105
- **Industry**: Municipal Services
- **Addressing Block**: 172.30.72.0/23
- **Networking Challenge**: DNS (Internal Name Resolution Service)

---

Client Requirements
1. Design a working computer network using Cisco Packet Tracer.
2. Implement an **Internal DNS Server** for name resolution.
3. **Separate VoIP traffic** from data traffic.
4. **Change Request (CR13)**: Implement a public kiosk with internet-only access.

---

 Network Design Summary
- **Topology**: Hierarchical Star with Centralized Routing (Router-on-a-stick).
- **Core Device**: Cisco 2911 Router, Cisco 3560 Core Switch.
- **VLANs**: Separated into Admin (VLAN 10), Staff (VLAN 20), VoIP (VLAN 30), Servers (VLAN 40), and Kiosk (VLAN 50).



| Subnet | Network | Mask | Gateway |
| :--- | :--- | :--- | :--- |
| Admin | 172.30.72.0/25 | 255.255.255.128 | 172.30.72.1 |
| Staff | 172.30.72.128/25 | 255.255.255.128 | 172.30.72.129 |
| VoIP | 172.30.73.0/26 | 255.255.255.192 | 172.30.73.1 |
| Servers | 172.30.73.64/28 | 255.255.255.240 | 172.30.73.65 |
| Kiosk | 172.30.73.80/28 | 255.255.255.240 | 172.30.73.81 |

---

 Repository Structure
- `/docs/` - Design documents, IP addressing, justifications.
- `/images/` - Screenshots of Packet Tracer topology and tests.
- `/configurations/` - Router and Switch configuration scripts.

---


---
 Student Information
- Siyabonga Nkosi
- 46499458
 28 August 2026
