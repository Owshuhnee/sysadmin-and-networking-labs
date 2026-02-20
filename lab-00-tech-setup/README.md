# Lab 00 — Technical Environment Setup

## Lab Metadata

- **Category:** Environment Setup  
- **Subdomain:** Virtualization / System Administration  
- **Difficulty:** Beginner  
- **Status:** Completed  
- **Host System:** Lenovo Yoga Pro 7 AMD
- **Last Updated:** February 21 2026  

---

## Objective

The objective of this lab is to prepare a stable technical environment for upcoming System Administration & Networking labs using virtualization.

This includes:

- Configuring the host operating system
- Installing virtualization software
- Deploying a Linux server virtual machine
- Verifying functionality by repeating previous lab tasks

---

## Background

Initially, the laptop was configured with a **dual-boot setup (Linux Mint + Windows 11)**.

However, persistent **Wi-Fi and network instability issues** occurred in Windows 11 after the dual-boot configuration. Multiple troubleshooting attempts were performed, but the issue could not be resolved reliably.

To ensure a stable learning environment and avoid further time loss, the system was reverted to:

> **Windows 11 as the primary and only operating system**

Virtualization was then selected as the preferred approach for running Linux environments.

This approach aligns with real-world industry practice where virtualization is commonly used for:

- Testing
- Lab environments
- Infrastructure simulation
- Safe experimentation

---

## Final Environment Architecture

### Host System

- **OS:** Windows 11 (Clean Installation)
- **Hardware:** Lenovo Yoga Pro 7
- **External Storage:** Crucial MX500 SSD (Lab Storage)

### Virtualization Layer

- **Hypervisor:** Oracle VirtualBox

### Guest System

- **Linux OS:** Ubuntu Server 24.04 LTS

---

## Software Installed

### Host Software

- Windows 11
- Oracle VirtualBox
- Git
- VS Code
- Cisco Packet Tracer

### Guest Software

- Ubuntu Server 24.04 LTS

---

## Virtual Machine Configuration

### Linux Server
| Component | Configuration |
|----------|---------------|
Memory | 8 GB RAM |
CPU | 4 Cores |
Disk | 60 GB (VDI) |
Network | NAT |
Graphics | Default |
EFI | Disabled |

---

## Storage Strategy

The external **Crucial MX500 SSD** is used as dedicated lab storage.
