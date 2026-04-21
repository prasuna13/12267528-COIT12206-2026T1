
# Week 01 Portfolio – GNS3 Introduction and Static IP Setup

**Name:** Prasuna Shrestha
**Student ID:** 12267528
**Unit:** COIT12206 TCP/IP Protocols  
**Week:** 01  
**Date:** 9/03/2026

---

## Objective
The objective of this task was to understand the unit requirements, set up the required tools, and practice basic GNS3 usage including configuring a Linux host with a static IP address.

---

## Tasks Completed
I reviewed the unit profile and confirmed the portfolio requirements, including maintaining a weekly GitHub repository using Markdown format. I ensured that GNS3 and VirtualBox were installed and working correctly.

I created a GNS3 project named **GNS3-Intro-<studentid>** and added a Linux Host node. I added annotations including my name, student ID, and project details. I configured a static IP address for the host using the `/etc/network/interfaces` file before starting the node.

After starting the node, I opened the console and verified the IP address using the `ip address show` command.

---

## Network Configuration
The network consisted of a single Linux Host with the following configuration:

- IP Address: 10.10.1.1  
- Subnet Mask: 255.255.255.0  
- Forwarding: Disabled  

Configuration used:

```bash
auto eth0
iface eth0 inet static
    address 10.10.1.1
    netmask 255.255.255.0
    up sysctl net.ipv4.ip_forward=0
## Screenshots / Evidence
![Network Topology](images/week01/network.png)
