# Lab 1 — Virtualisation Fundamentals

## Lab Metadata
- **Category:** System Administration
- **Subdomain:** Virtualisation
- **Difficulty:** Beginner
- **Status:** Completed
- **Estimated Time:** 2–3 hours

---

## Objective
The goal of this lab was to gain hands-on experience with virtualisation fundamentals by creating and managing a Linux virtual machine. The lab focuses on understanding how virtual machines are provisioned, isolated, and recovered using snapshots.

This lab establishes a foundation for later System Administration and Cybersecurity labs by providing a safe, repeatable environment for testing and experimentation.

---

## Environment
- **Host OS:** Windows 11
- **Hypervisor:** VirtualBox
- **Guest OS:** Ubuntu Server 22.04 LTS
- **Networking Mode:** NAT
- **Hardware Allocation:**
  - CPU: 2 cores
  - RAM: 4 GB
  - Storage: 30 GB (VDI)

---

## Tasks Performed

1. Installed VirtualBox on the host system  
2. Created a new virtual machine  
3. Installed Ubuntu Server using manual configuration  
4. Configured networking using NAT  
5. Enabled and tested SSH access  
6. Took and restored VM snapshots  
7. Verified system status using basic Linux commands  

---

## Evidence
Screenshots are provided to demonstrate:
- Virtual machine configuration  
- Ubuntu Server installation progress  
- Successful login and system information  
- SSH connectivity confirmation  
- Snapshot creation and restore  

## Screenshots
- [01 – VirtualBox installed](./screenshots/01-virtualbox-installed.png)
- [02 – VM hardware summary](./screenshots/02-vm-hardware-summary.png)
- [03 – Network adapter (NAT)](./screenshots/03-network-adapter-nat.png)
- [04 – Ubuntu boot menu](./screenshots/04-ubuntu-boot-menu.png)
- [05 – Installation type](./screenshots/05-installation-type.png)
- [06 – Network (DHCP)](./screenshots/06-network-dhcp.png)
- [07 – Storage (LVM summary)](./screenshots/07-storage-lvm-summary.png)
- [08 – Profile configuration](./screenshots/08-profile-configuration.png)
- [09 – First login](./screenshots/09-first-login.png)
- [10 – SSH enabled](./screenshots/10-ssh-enabled.png)
- [11 – Clean install snapshot](./screenshots/11-clean-install-snapshot.png)

---

## Key Concepts Learned
- **Virtual Machines (VMs):** Isolated environments running on shared hardware  
- **Hypervisors:** Software used to create and manage VMs  
- **NAT Networking:** Provides outbound connectivity while maintaining isolation  
- **Snapshots:** Point-in-time VM states for quick recovery  
- **SSH:** Secure remote access to a server  

---

## Security Considerations
- SSH access was enabled only when required  
- Default credentials were avoided  
- Network isolation was maintained using NAT  
- Snapshot usage helps recover from misconfiguration or compromise  

---

## Reflection
This lab helped build my confidence working with virtual machines and Linux servers. Doing a manual installation gave me a better understanding of system configuration compared to automated setups, and managing snapshots highlighted how important backups and recovery are in system administration.

The lab also felt a bit easier because I’ve worked with Hyper-V before during my Certificate in Information Technology. I had prior experience creating both host and local virtual machines, including Windows Server 2022 environments, which made the concepts easier to follow this time around.

Compared to the sandbox labs I used previously, running everything locally in VirtualBox was a much smoother experience. Things clicked faster, and the overall process made more sense.

This lab also helped me properly understand snapshots. I can now see how VirtualBox snapshots are essentially the same concept as Hyper-V checkpoints, just implemented on a different platform.

---


## Next Steps
- Prepare for Lab 2: Linux User & Group Management 
