# 🧠 WGU Capstone: Enterprise Network Simulation (Cisco Packet Tracer)

This project was developed as the final capstone for the **B.S. in Network Engineering and Security** at **Western Governors University**.  
It simulates an enterprise-grade network for a fictional company — **TrueCover Insurance Solutions** — using **Cisco Packet Tracer**, based on real-world networking principles and security standards.

## 🏢 Scenario Overview

TrueCover Insurance operates with 10 employees across two main departments (IT and Sales), along with guest users like consultants and clients.  
The network must maintain **reliable access**, **strong segmentation**, **redundancy**, and **secure external connectivity**, while aligning with business needs and security compliance.

---

## ✅ Project Features

The network design satisfies all **10 required test cases** listed below.

| Test Case | Requirement | Implementation Summary |
|-----------|-------------|-------------------------|
| **#1**: Device Discovery & Reachability | Multiple network segments and access controls | Devices in each VLAN are restricted from accessing other VLANs; routing and ACLs ensure isolation. |
| **#2**: Access Control for Guest Access | Limit guest access to internet traffic only | ACLs applied to guest VLAN restrict internal resource access, only allowing external (internet) access. |
| **#3**: Security Compliance – Log-in Banners | Notify users of acceptable use policy (AUP) | Banner messages set on all routers and switches to display AUP at login. |
| **#4**: Routing & External Traffic | Proper IP addressing, DHCP, and static IP use | End-user devices get IPs via DHCP; web and server resources use static IPs. |
| **#5**: Layer 2 Redundancy (STP) | Prevent loops and ensure path reliability | STP (802.1w) is enabled on switches; root bridge manually configured to manage spanning tree behavior. |
| **#6**: Syslog & NTP | Generate system logs and use time synchronization | Edge routers forward logs to a Syslog server and sync with an internal NTP server. |
| **#7**: Layer 2 Segmentation via VLANs | VLANs for departments to reduce congestion | Separate VLANs created for IT, Sales, and Guests. VLAN trunking configured on uplinks. |
| **#8**: EtherChannel | Link aggregation for bandwidth and redundancy | EtherChannel is configured between core switches using LACP to improve throughput and failover. |
| **#9**: Remote Access | Secure SSH access to devices | SSH enabled on all routers for encrypted remote administration; passwords and key authentication set. |
| **#10**: Network Security | Port security for guest switch ports | MAC address limiting enforced on guest VLAN ports to block unauthorized endpoint connections. |

---

## 🧰 Technologies Used

- **Cisco Packet Tracer**
- VLANs, Inter-VLAN Routing, DHCP
- ACLs, SSH, Port Security
- Spanning Tree Protocol (STP)
- EtherChannel (LACP)
- Syslog & NTP
- Static and Dynamic IP Addressing

---

## 📄 Files Included

- `Capstone Functionality Report Packet Tracer.pdf` – full technical report with configuration proof, test case mapping, and validation screenshots.

