## Task 4 — Implement Least-Privilege Sudo Access (Pending)

### User Story
As an administrator, I want developers to run limited administrative commands without granting full sudo access.

---

### Acceptance Criteria
- [ ] `sudo -l` shows only approved commands
- [ ] Privilege escalation beyond scope is denied
- [ ] System integrity remains intact

---

### Scope of Elevated Access

**Allowed**
- Developers can check the status of the application service
- Developers can restart the application service

**Not Allowed**
- Full administrative (sudo) access
- User, group, or system configuration changes

---

### User Roles & Sudo Policy
The following users and sudo access rules were defined:

- **jove** (Primary Admin)  
  Full sudo access

- **alex-dev** (Developer)  
  Limited sudo access for specific application-related commands only

- **mika-qa** (QA)  
  No sudo access

- **sam-intern** (Intern)  
  No sudo access

---

### Tasks Performed

#### Defining the Policy
A least-privilege sudo policy was designed so that developers can perform basic operational tasks (such as restarting or checking the status of the application service) without being able to fully administer the system.

---

#### Verifying Sudo Access

**jove (Primary Admin)**  
Full sudo access was verified successfully.

![Verify sudo access — jove](./screenshots/23-verify-sudo-main.png)

---

**alex-dev (Developer)**  
When initially testing sudo access as `alex-dev`, I was prompted for a password. I first attempted to use the primary admin (`jove`) password, which failed. I thought that its the password for every user as jove was the main admin. I learned that sudo authentication requires the **target user’s own password** and not another user’s credentials.

After setting a password for `alex-dev`, sudo access was tested again.

![Verify sudo access — alex-dev](./screenshots/24-verify-sudo-alex-dev.png)

---

### Commands Used
```bash
sudo -l
sudo passwd user
``` 

---

### References/Learning Aid
- [Linux Crash Course - sudo](https://www.youtube.com/watch?v=07JOqKOBRnU)