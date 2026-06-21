# SOHO Network Design & Implementation Using Cisco Packet Tracer

## Project Overview

This project demonstrates the design and implementation of a Small Office/Home Office (SOHO) network using Cisco Packet Tracer. The objective is to build a segmented and functional network for a small organization, ensuring proper separation of departments, controlled communication, and efficient IP address management.

The network represents a real-world enterprise branch environment with three departments:

* Admin / IT
* Finance / HR
* Customer Service / Reception

---

## Key Technologies Used

* VLANs for network segmentation
* Router-on-a-Stick for inter-VLAN routing
* DHCP for automatic IP address allocation
* IPv4 subnetting for efficient address planning
* Cisco IOS command-line configuration
* Wireless networking for client connectivity

---

## Network Design

The network is divided into three VLANs, each representing a separate department. This ensures logical isolation of traffic while maintaining controlled communication between departments through routing.

Base Network: 192.168.1.0/26

| Department       | VLAN | Network Address | Host Range          | Gateway       |
| ---------------- | ---- | --------------- | ------------------- | ------------- |
| Admin / IT       | 10   | 192.168.1.0     | 192.168.1.1 – 62    | 192.168.1.1   |
| Finance / HR     | 20   | 192.168.1.64    | 192.168.1.65 – 126  | 192.168.1.65  |
| Customer Service | 30   | 192.168.1.128   | 192.168.1.129 – 190 | 192.168.1.129 |

---

## Implementation Summary

### VLAN Segmentation

Each department is assigned a dedicated VLAN to isolate network traffic and improve security and performance.

### Inter-VLAN Routing

A router-on-a-stick configuration is used to enable communication between VLANs while maintaining logical separation.

### DHCP Configuration

A DHCP server is configured on the router to automatically assign IP addresses to all end devices within each VLAN.

### Wireless Connectivity

Access points are deployed to provide wireless access to users within each department.

---

## Testing and Verification

The following tests were performed to validate the network:

* Successful communication within and between VLANs
* DHCP-based automatic IP assignment
* Proper routing between different network segments
* Wireless client connectivity
* End-to-end connectivity using ping tests

---

## Skills Demonstrated

* VLAN configuration and network segmentation
* Inter-VLAN routing using router-on-a-stick
* IPv4 addressing and subnetting
* DHCP configuration and management
* Cisco IOS command-line usage
* Basic wireless network setup
* Network troubleshooting and validation

---

## Conclusion

This project successfully demonstrates a functional SOHO network that reflects real-world enterprise networking principles. It shows how network segmentation, routing, and automation can be used to build a structured, scalable, and efficient small business network using Cisco Packet Tracer.
