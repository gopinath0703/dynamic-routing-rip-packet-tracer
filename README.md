# Dynamic Routing using RIP - Cisco Packet Tracer

## 📋 Project Overview
A 3-router network topology designed and configured with RIP 
(Routing Information Protocol) to enable dynamic route sharing 
across three subnets.

## 🖥️ Topology
- 3 Routers (WAN links via Serial interfaces)
- 3 Layer 2 Switches (2960-24TT)
- 6 End devices (2 PCs per subnet)

## 🌐 IP Addressing

| Network | Subnet | Router Interface |
|---------|--------|-------------------|
| LAN 1 | 192.168.1.0/24 | Router1 Fa0/0 |
| LAN 2 | 192.168.2.0/24 | Router2 Fa0/0 |
| LAN 3 | 192.168.3.0/24 | Router3 Fa0/0 |
| WAN Link 1 | 10.0.0.0/30 | Router1 - Router2 |
| WAN Link 2 | 11.0.0.0/30 | Router2 - Router3 |

## ⚙️ Configuration Highlights
- Configured RIP version 2 on all routers
- Advertised connected networks using the `network` command
- Configured serial interfaces with clock rate on DCE end
- Verified routing table using `show ip route`

## ✅ Verification
- 100% successful ICMP ping across all subnets
- RIP routes (D) visible in routing table confirming dynamic 
  route propagation

## 🛠️ Tools Used
Cisco Packet Tracer 8.2.2

## 📁 Files
- `Dynamic Routing rip Version 1.pkt` - Packet Tracer project file
- `screenshots/` - Topology and verification screenshots
