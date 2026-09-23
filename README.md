 Enterprise Network Design & Implementation

A multi-department enterprise network designed and implemented using Cisco Packet Tracer.

## 📌 Project Overview

This project demonstrates the design, configuration, routing, services, security, and troubleshooting of an enterprise LAN environment.

The network is divided into multiple departments using VLANs and uses a Layer-3 Core Switch for inter-VLAN routing.

## 🏗️ Network Topology

The network contains:

- Cisco 2911 Edge Router
- Cisco 3560 Layer-3 Core Switch
- 5 × Cisco 2960 Access Switches
- 8 × PCs
- 3 × Servers

### Departments

- HR
- Finance
- IT
- Management
- Server Network

## 🌐 VLAN & IP Addressing

| VLAN | Department | Network | Gateway |
|------|------------|---------|---------|
| 10 | HR | 192.168.10.0/24 | 192.168.10.1 |
| 20 | Finance | 192.168.20.0/24 | 192.168.20.1 |
| 30 | IT | 192.168.30.0/24 | 192.168.30.1 |
| 40 | Management | 192.168.40.0/24 | 192.168.40.1 |
| 50 | Servers | 192.168.50.0/24 | 192.168.50.1 |

## 🔧 Technologies & Concepts

- Cisco Packet Tracer
- VLAN
- 802.1Q Trunking
- Layer-3 Switching
- Inter-VLAN Routing
- SVI
- DHCP
- DHCP Relay
- DNS
- HTTP
- Static Routing
- Default Routing
- Basic Switch Security
- Network Troubleshooting

## 🖥️ Server Services

### DHCP Server
IP Address: 192.168.50.10

Provides IP configuration to client VLANs.

### DNS Server
IP Address: 192.168.50.11

DNS record:

intranet.company.local → 192.168.50.12

### Web Server
IP Address: 192.168.50.12

Internal website:

http://intranet.company.local

## 🚦 Routing

The Core Switch performs inter-VLAN routing using SVIs.

The Core-to-Router transit network is:

10.0.0.0/30

- R1-EDGE: 10.0.0.1
- SW-CORE: 10.0.0.2

Static and default routing were configured between the Core Switch and Edge Router.

## 🔐 Security

Basic switch security was configured using:

- Enable Secret
- Console Password
- VTY Password
- Password Encryption

> Credentials are not published in this repository.

## 🧪 Verification & Testing

The following commands were used for verification:

```text
show vlan brief
show interfaces trunk
show ip interface brief
show ip route
ping
Testing included:

VLAN connectivity

Inter-VLAN connectivity

DHCP address assignment

DNS name resolution

Internal Web Server access

Router/Core connectivity

📁 Project Files
Enterprise_Network_Cisco_Packet_Tracer.pkt — Complete Packet Tracer project

README.md — Project documentation

🎯 Learning Outcomes
Through this project I practiced:

Enterprise network design

VLAN segmentation

Layer-3 switching

Routing

DHCP and DNS services

Network troubleshooting

Cisco CLI configuration

Basic network security

👨‍💻 Author
Kumar

Interested in:

IT Support

Networking

Cloud Computing

Infrastructure
