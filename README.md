# 🌐 Network Monitoring & Troubleshooting Lab

A Cisco Packet Tracer project focused on **network monitoring, fault detection, troubleshooting, routing, switching, and secure network management**.

## 📌 Project Overview

This project simulates an enterprise network where network engineers can monitor devices, identify connectivity problems, introduce controlled network failures, troubleshoot them using Cisco IOS commands, and verify the recovery.

The main workflow is:

**Detect → Analyze → Troubleshoot → Fix → Verify**

---

## 🎯 Objectives

- Design an enterprise network
- Configure VLANs and trunking
- Implement Inter-VLAN Routing
- Configure DHCP
- Implement OSPF dynamic routing
- Configure SSH for secure management
- Implement Syslog monitoring
- Configure NTP synchronization
- Configure SNMP
- Introduce network faults
- Troubleshoot network failures
- Verify network recovery

---

## 🛠️ Technologies Used

- Cisco Packet Tracer
- Cisco IOS
- VLAN
- IPv4
- Subnetting
- Trunking
- Layer-3 Switching
- Inter-VLAN Routing
- DHCP
- OSPF
- SSH
- Syslog
- NTP
- SNMP
- Network Troubleshooting

---

## 🖥️ Network Devices

| Device | Model | Quantity |
|---|---|---:|
| Router | Cisco 2911 | 2 |
| Layer-3 Switch | Cisco 3560 | 1 |
| Access Switch | Cisco 2960 | 3 |
| PCs | PC-PT | 6 |
| Servers | Server-PT | 2 |

---

## 🌐 IP Addressing

| VLAN | Name | Network | Gateway |
|---|---|---|---|
| 10 | USERS | 192.168.10.0/24 | 192.168.10.1 |
| 20 | IT | 192.168.20.0/24 | 192.168.20.1 |
| 30 | SERVERS | 192.168.30.0/24 | 192.168.30.1 |

### WAN

| Device | Interface | IP |
|---|---|---|
| CORE-R1 | S0/0/0 | 10.0.0.1/30 |
| ISP-R2 | S0/0/0 | 10.0.0.2/30 |

---

## 🔀 VLAN Configuration

### VLAN 10 — USERS

Used for general users.

### VLAN 20 — IT

Used for IT/network administration.

### VLAN 30 — SERVERS

Used for monitoring and internal services.

---

## 🚦 Inter-VLAN Routing

The Cisco 3560 Layer-3 switch performs routing between VLANs using SVIs.

```text
VLAN 10 → 192.168.10.1
VLAN 20 → 192.168.20.1
VLAN 30 → 192.168.30.1
