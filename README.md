# Radeon Company Enterprise Network Infrastructure Design

## Overview

This project demonstrates the design and implementation of a scalable enterprise network infrastructure for Radeon Company Ltd., a United States-based Banking and Insurance organization expanding operations into Africa with its first regional branch located in Nairobi, Kenya.

The solution was developed using Cisco Packet Tracer and follows industry-standard enterprise networking practices including hierarchical network architecture, VLAN segmentation, dynamic routing, centralized services, wireless networking, and network redundancy.

The network was designed to support multiple departments distributed across four floors while ensuring scalability, availability, and efficient communication throughout the organization.

---

## Business Scenario

Radeon Company Ltd. is establishing a new regional office in Nairobi, Kenya to support its African operations.

The company acquired a four-story office building and requires a modern enterprise network infrastructure capable of supporting:

* Banking Operations
* Insurance Services
* Internal Business Applications
* Wireless Connectivity
* Centralized Network Services
* Future Business Growth

The network was designed to provide secure communication between all departments while maintaining proper segmentation and centralized management.

---

## Building Structure

### First Floor

#### Management Department

* 20 PCs
* 4 Printers

#### Research Department

* 20 PCs
* 4 Printers

#### Human Resources Department

* 20 PCs
* 4 Printers

---

### Second Floor

#### Marketing Department

* 20 PCs
* 4 Printers

#### Accounting Department

* 20 PCs
* 4 Printers

#### Finance Department

* 20 PCs
* 4 Printers

---

### Third Floor

#### Logistics and Store Department

* 20 PCs
* 4 Printers

#### Customer Care Department

* 20 PCs
* 4 Printers

#### Guest Area

* 20 PCs
* 2 Printers

---

### Fourth Floor

#### Administration Department

* 20 PCs
* 2 Printers

#### ICT Department

* 20 PCs
* 2 Printers

#### Server Room

Infrastructure:

* DHCP Server
* Web Server
* Email Server
* Administrative Workstations

---

## Network Architecture

The design follows a three-tier hierarchical enterprise model.

### Core Layer

Responsible for:

* High-speed backbone connectivity
* Routing between floors
* OSPF route propagation

### Distribution Layer

Responsible for:

* VLAN routing
* Policy enforcement
* Aggregation of access switches

### Access Layer

Responsible for:

* End-user connectivity
* Department switches
* Wireless access points

---

## Technologies Implemented

### Enterprise Network Design

* Hierarchical Network Architecture
* Redundant Network Design
* Multi-Floor Enterprise Deployment

### Routing Technologies

* OSPF Dynamic Routing
* Router-to-Router Communication

### Switching Technologies

* VLAN Segmentation
* Inter-VLAN Communication

### Network Services

* DHCP Services
* HTTP Web Services
* Email Services

### Wireless Technologies

* Department Wireless Networks
* Cisco Wireless Access Points

### Management Technologies

* SSH Remote Administration
* Device Hardening

---

## VLAN Design

Each department was assigned an independent VLAN.

| VLAN     | Department          |
| -------- | ------------------- |
| VLAN 10  | Management          |
| VLAN 20  | Research            |
| VLAN 30  | Human Resources     |
| VLAN 40  | Marketing           |
| VLAN 50  | Accounting          |
| VLAN 60  | Finance             |
| VLAN 70  | Logistics and Store |
| VLAN 80  | Customer Care       |
| VLAN 90  | Guest Area          |
| VLAN 100 | Administration      |
| VLAN 110 | ICT                 |
| VLAN 120 | Server Room         |

---

## IP Addressing Plan

### Base Network

192.168.10.0/24

Subnetting was performed using VLSM to allocate address space efficiently across departments while supporting both wired and wireless users.

### Routing Network

10.10.10.0/24

Used for router-to-router communication and routing infrastructure.

---

## Services Implemented

### DHCP Server

Provides:

* Dynamic IPv4 Address Allocation
* Default Gateway Distribution
* DNS Information Distribution

### HTTP Server

Provides:

* Internal Company Website
* Web-Based Services

### Email Server

Provides:

* Internal Organizational Email Communication

---

## Routing Design

OSPF was deployed across all routing devices to provide:

* Dynamic Route Advertisement
* Fast Convergence
* Scalable Network Expansion

All routers participate in OSPF and exchange routes automatically.

---

## Wireless Infrastructure

Each department contains a dedicated wireless network allowing users to connect through:

* Laptops
* Smartphones
* Wireless Workstations

The wireless deployment complements the wired infrastructure while maintaining departmental segmentation.

---

## Security Features

### SSH Remote Management

SSH was configured on all routers to provide:

* Encrypted Remote Access
* Secure Device Administration

### Device Hardening

Implemented:

* Hostnames
* Console Passwords
* VTY Passwords
* Enable Secrets
* Login Banners
* Disabled DNS Lookup

---

## Testing and Verification

The following tests were successfully completed:

* DHCP Address Assignment
* OSPF Neighbor Formation
* Same VLAN Communication
* Inter-VLAN Communication
* End-to-End Connectivity
* HTTP Server Access
* Email Server Communication
* SSH Remote Login
* Wireless Connectivity Testing

All configured services were tested and verified successfully.

---

## Skills Demonstrated

* Enterprise Network Design
* Hierarchical Architecture Design
* VLAN Segmentation
* Inter-VLAN Routing
* OSPF Routing
* DHCP Administration
* Email Server Deployment
* Web Server Deployment
* Wireless Network Design
* SSH Configuration
* Enterprise Documentation
* Cisco Packet Tracer
* Network Troubleshooting

---

## Repository Structure

```text
radeon-enterprise-network/
│
├── README.md
├── Radeon_Enterprise_Network.pkt
├── Radeon_Project_Report.pdf
├── topology.png

---

## Author

Chibuike Obika

Enterprise Network Engineering Portfolio Project
