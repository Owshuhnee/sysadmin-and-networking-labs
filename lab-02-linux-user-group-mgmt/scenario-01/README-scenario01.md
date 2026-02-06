# Lab 2 — Linux User & Group Management

## Lab Metadata
- **Category:** System Administration
- **Subdomain:** Linux Administration
- **Difficulty:** Beginner
- **Mode:** Scenario was AI generated
- **Status:** In Progress
- **Estimated Time:** (pending)

---

## Scenario Overview

You are acting as a **Junior Linux System Administrator** in a small organization.  
A new internal application project is starting, and you are responsible for:

- Onboarding users
- Managing group-based access
- Enforcing least privilege
- Troubleshooting permission issues
- Offboarding users cleanly

All access must be controlled through **groups and permissions**, not per-user exceptions.

---

## Environment
- **Host OS:** Windows 11
- **Hypervisor:** VirtualBox
- **Guest OS:** Ubuntu Server 22.04 LTS
- **Lab VM:** Keep Lab 2 users/groups and create new ones for this scenario

---

## Roles & Access Model

| Role | Purpose | Access Summary |
|-----|--------|----------------|
| sysadmin | Full system administration | Full sudo |
| devs | Application deployment | Write to app directory, limited sudo |
| qa | Testing and verification | Read-only access to logs |
| interns | Training only | Restricted training directory |

---

## Tasks
- [Task 1 — Group / Role Management](./task-01.md)
- [Task 2 — User Management](./task-02.md)
- [Task 3 — Shared Directories & Permissions](./task-03.md)
- [Task 4 — Least-Privilege Sudo Access](./task-04.md)
- [Task 5 — Incident Response: Permission Denied](./task-05.md)

---

## Lessons Learned

In this lab I learned how Linux access control is primarily driven by **group ownership and directory permissions** (not individual users). I learned how important it is to think about the entire directory path when troubleshooting permission issues, as access can be blocked by parent directories even when target permissions appear correct.

Implementing least-privilege sudo access highlighted how powerful and flexible sudo rules can be when applied at the group level rather than per user. This approach scales better and reduces the risk of over-permissioning.

Finally, the offboarding task showed the value of handling user removal in a controlled and auditable way. Locking accounts instead of deleting them immediately preserves system data for review while still preventing access, which reflects real-world system administration practices.

