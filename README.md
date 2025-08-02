# VLAN Simulation Lab (Packet Tracer)

## 🎯 Objective
Design and configure:
- 3 VLANs: Management, Production, Guest
- Trunk port between switch and router
- Inter-VLAN routing (Router-on-a-Stick)
- Test connectivity across VLANs

## 🛠️ Topology
<img width="858" height="540" alt="basic topology" src="https://github.com/user-attachments/assets/ac133d6e-14ec-4f54-bab0-e2556cb4d5ad" />


Devices:
- Router: R1
- Switch: SW-Core
- PCs: PC-Mgmt, PC-Prod, PC-Guest

## 🧩 VLANs
| VLAN | Name        | Subnet            | Gateway          |
|------|-------------|-------------------|------------------|
| 10   | Management  | 192.168.10.0/24   | 192.168.10.1     |
| 20   | Production  | 192.168.20.0/24   | 192.168.20.1     |
| 30   | Guest       | 192.168.30.0/24   | 192.168.30.1     |

## ⚙️ Configuration Highlights
- Switch ports assigned per VLAN
- Router subinterfaces with 802.1Q encapsulation
- Trunk on Fa0/24

## ✅ Testing
All devices can ping each other across VLANs.
<img width="685" height="753" alt="ping success between different VLANs" src="https://github.com/user-attachments/assets/c054a361-be2f-4926-975f-a8b86e2047a5" />


## 💾 File
- `vlan-lab.pkt`: Packet Tracer file
