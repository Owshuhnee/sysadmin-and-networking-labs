# Lab 00 — Tech Stack & Environment Setup

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

---

## Tasks Performed

### 1. Reinstalled Windows 11 (Clean Installation)

- Removed previous dual-boot configuration
- Installed Windows 11 as single OS
- Updated drivers and system packages

### 2. Installed VirtualBox

- Installed Oracle VirtualBox
- Installed Extension Pack
- Verified virtualization support in BIOS

### 3. Created Ubuntu Server Virtual Machine

- Created VM with custom hardware configuration
- Mounted Ubuntu Server ISO
- Installed OS manually
- Configured user credentials

### 4. Verified Environment

To confirm the environment works correctly:

- Repeated tasks from **Lab 02 (Linux Users & Groups)**
- Confirmed:
  - User creation
  - Group management
  - Permissions
  - Sudo access

This validated the VM environment is stable and functional.

---


## Challenges Encountered

### Issue: Windows Wi-Fi instability after dual-boot

**Symptoms:**

- Slow internet speeds
- Disconnections
- Network errors
- Driver inconsistencies

**Resolution:**

- Removed Linux dual-boot
- Reinstalled Windows cleanly
- Switched to virtualization approach

---

## Security Considerations

- Virtual machines provide isolation from host system
- Snapshots allow safe experimentation
- External storage allows backup separation
- Reduced risk compared to modifying host partitions

---

## Reflection

The initial plan to use a dual-boot configuration introduced unexpected system instability, particularly affecting network performance on Windows 11. Troubleshooting consumed significant time with limited results.

Reverting to a **Windows-only host with virtualization** proved to be a more efficient and stable approach.

This experience reinforced an important real-world lesson:

> Stability and reliability are more valuable than theoretical optimization.

Virtualization provides flexibility, safety, and faster recovery, making it ideal for learning environments.

---

## Next Steps

Resume:
Lab 03 - Linux Networking
Cisco Networking Academy - Networking basics
Practice Simulations with Cisco packet tracer

---

## Status

Environment successfully prepared and validated ✅