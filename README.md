# 🧪 Basic Cisco Router and Switch Configuration Lab (Packet Tracer)

This project was completed as part of a cybersecurity training fellowship. The goal was to simulate a small business network using Cisco Packet Tracer, configure a router and two switches with secure remote access, and verify device-to-device connectivity using CLI tools. All configurations and IP assignments were implemented manually and tested for proper functionality.

---

## 🎯 Lab Objectives

- Build a network using a Cisco 2911 router, two 2960 switches, and four PCs
- Configure interfaces, IP addresses, and default gateways
- Apply basic security to all devices (console, VTY, AUX passwords)
- Enable remote management via VLAN 1 on both switches
- Verify connectivity using CLI commands and Packet Tracer tools

---

## 🧱 Network Design

| Subnet | IP Range           | Devices                         |
|--------|--------------------|---------------------------------|
| A      | 192.168.1.0/24     | PC0, PC1, Switch0, Router G0/0  |
| B      | 192.168.2.0/24     | PC2, PC3, Switch1, Router G0/1  |

---

### 🖼️ Topology Diagram



---

## 🧰 Devices Used

- 1x Cisco 2911 Router
- 2x Cisco 2960 Switches
- 4x Generic PCs
- 6x Copper Straight-Through Cables

---

## 💻 PC IP Settings

| PC   | IP Address      | Subnet Mask     | Default Gateway   |
|------|------------------|------------------|--------------------|
| PC0  | 192.168.1.10     | 255.255.255.0    | 192.168.1.1        |
| PC1  | 192.168.1.11     | 255.255.255.0    | 192.168.1.1        |
| PC2  | 192.168.2.10     | 255.255.255.0    | 192.168.2.1        |
| PC3  | 192.168.2.11     | 255.255.255.0    | 192.168.2.1        |

---

## ⚙️ Configuration Files

- [📄 router-config.txt](./router-config.txt) – Cisco 2911 router configuration
- [📄 switch0-config.txt](./switch0-config.txt) – Switch0 VLAN and security config
- [📄 switch1-config.txt](./switch1-config.txt) – Switch1 VLAN and security config

---

## ✅ Verification & Troubleshooting Commands

These are included across the `.txt` files and should be used in the CLI to validate connectivity:

| Command                      | Purpose                                          |
|-----------------------------|--------------------------------------------------|
| `ping [IP_ADDRESS]`         | Test connectivity between PCs, router, switches |
| `show ip interface brief`   | Verify IP address and interface status           |
| `show running-config`       | View active configuration                        |
| `show interfaces status`    | Check switch port status                         |
| `show vlan brief`           | See VLAN assignment and port mapping             |
| `show clock`                | Display system clock (timezone config test)      |
| `show mac address-table`    | Display MAC learning status on switches          |

---

## 🛠️ Created With

- [Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer)
- Cisco IOS CLI

