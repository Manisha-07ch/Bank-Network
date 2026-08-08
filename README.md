# Secure_Bank_Network

# 🏦 Secure Banking Network Design & Implementation

## 📌 Project Overview

This project presents the design and implementation of a **Secure Banking Network** using Cisco networking technologies and Cisco Packet Tracer.

The network is designed to provide:

- 🔐 Secure communication
- 🌐 Reliable branch connectivity
- 🏢 Departmental network segmentation
- 🔄 Network redundancy
- 🛡️ Access control and security
- 📡 WAN connectivity
- 🖥️ Centralized banking server connectivity
- 📊 Network monitoring and troubleshooting

The topology consists of a **central Secure Banking Core** connected to **two remote branches**.

---

## 🎯 Project Objectives

The main objectives of this project are:

1. Design a secure enterprise banking network.
2. Connect multiple departments using network segmentation.
3. Provide reliable communication between branches and the central office.
4. Implement routing between different networks.
5. Provide redundancy for critical network infrastructure.
6. Control network access using security policies and ACLs.
7. Secure access to banking servers.
8. Test connectivity and troubleshoot network problems.
9. Create a scalable architecture for future expansion.

---

## 🏗️ Network Architecture

The network consists of the following major sections:

### 🏢 Central Banking Core

The central banking network contains:

- Primary Edge Router
- Backup Edge Router
- Core/Distribution Switches
- Banking Servers
- Operations Department
- Finance Department
- Customer Service Department
- IT Administration Department

### 🏦 Branch 1

Branch 1 contains:

- Cisco 2911 Router
- Cisco 2960 Switch
- Teller Workstation
- WAN connection to the central banking network

### 🏦 Branch 2

Branch 2 contains:

- Cisco 2911 Router
- Cisco 2960 Switch
- Teller Workstation
- WAN connection to the central banking network

---

## 🌐 Network Topology

https://github.com/user-attachments/assets/b9d59b3b-4887-42dc-b299-ba4588efdc36

> The topology above represents the logical design of the Secure Banking Network implemented in Cisco Packet Tracer.

---

## 📊 IP Addressing Scheme

| Network/Department | Network Address | Subnet Mask | Purpose |
|---|---|---|---|
| Operations | 192.168.10.0/24 | 255.255.255.0 | Operations Department |
| Finance | 192.168.20.0/24 | 255.255.255.0 | Finance Department |
| Customer Service | 192.168.30.0/24 | 255.255.255.0 | Customer Service |
| IT Administration | 192.168.40.0/24 | 255.255.255.0 | IT Administration |
| Banking Servers | 192.168.50.0/24 | 255.255.255.0 | Banking Servers |
| Branch 1 LAN | 192.168.110.0/24 | 255.255.255.0 | Branch 1 |
| Branch 2 LAN | 192.168.120.0/24 | 255.255.255.0 | Branch 2 |
| WAN Links | 10.0.0.0/30 etc. | 255.255.255.252 | Point-to-Point WAN |

---

## 🔀 VLAN Segmentation

Network segmentation is used to separate different departments.

| VLAN | Department | Network |
|---:|---|---|
| 10 | Operations | 192.168.10.0/24 |
| 20 | Finance | 192.168.20.0/24 |
| 30 | Customer Service | 192.168.30.0/24 |
| 40 | IT Administration | 192.168.40.0/24 |
| 50 | Banking Servers | 192.168.50.0/24 |

### Benefits

- Reduces broadcast traffic
- Improves security
- Provides logical separation
- Makes access control easier
- Limits unauthorized lateral movement
- Simplifies network management

---

## 🚦 Routing

Routing is used to provide communication between:


Operations
     ↕
Finance
     ↕
Customer Service
     ↕
IT Administration
     ↕
Banking Servers
     ↕
Branch 1
     ↕
Branch 2
