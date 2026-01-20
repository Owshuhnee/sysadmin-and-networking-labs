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
  - Storage: 40 GB (VDI)

---

## Tasks Performed

1. Installed and configured VirtualBox on the host system  
2. Created a new Ubuntu Server virtual machine  
3. Configured CPU, memory, and storage settings  
4. Set up NAT networking for outbound connectivity  
5. Installed Ubuntu Server from ISO  
6. Verified network connectivity and system access  
7. Created and restored a VM snapshot to simulate recovery  

---

## Evidence
Screenshots are provided to demonstrate:
- Virtual machine configuration
- Successful OS installation
- Network connectivity
- Snapshot creation and restore process

📁 **Screenshots:** `./screenshots/`

---

## Key Concepts Learned
- Difference between host and guest operating systems
- Role of a hypervisor in resource isolation
- Benefits of virtualisation for testing and learning
- Snapshot usage for rollback and disaster recovery
- Importance of consistent environments in system administration

---

## Security Considerations
- Virtual machines provide isolation from the host system, reducing risk during experimentation
- NAT networking limits direct inbound access to the VM
- Snapshots allow recovery from misconfiguration or compromise
- Resource limits help prevent denial-of-service scenarios on the host

---

## Reflection
This lab reinforced the importance of virtualisation as a core system administration skill. Being able to quickly deploy, snapshot, and recover systems enables safe learning and efficient troubleshooting.

These skills will be reused throughout future labs involving user management, networking services, and security hardening.

---

## Next Steps
- Expand VM usage with multiple users and groups
- Introduce bridged networking for advanced scenarios
- Use this VM as a base system for future labs
