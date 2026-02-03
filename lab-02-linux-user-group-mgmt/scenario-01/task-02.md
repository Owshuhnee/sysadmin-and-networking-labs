## Task 2 — User Management

### User Story
As an administrator, I want new staff accounts created with correct group membership and secure defaults.

---

### Acceptance Criteria
- [x] Users exist and can log in  
- [x] Correct primary and secondary groups assigned  
- [x] Home directories exist with correct ownership  
- [x] No administrative access granted unintentionally  

---

### Tasks Performed
To reduce naming confusion and better reflect role intent, the existing administrative user `jove-admin` was renamed to `mark-admin`. During this process, I learned that Linux does **not** automatically update a user’s primary group name or home directory when a username is changed. These components must be handled separately to maintain consistency.

The update was completed in three steps, as shown in the screenshot below.

![Modify Admin User](./screenshots/06-modify-admin-user.png)

After confirming that the administrative account was correctly updated, additional role-based users were created for the environment. Each user was created with a home directory and default shell, then validated to ensure correct UID, GID, group membership, and home directory ownership.

- **Developers:** `alex-dev`  
- **QA:** `mika-qa`  
- **Interns:** `sam-intern`  

![Add Users](./screenshots/07-create-users-success.png)  
![Verify Users & Groups](./screenshots/08-verify-uid-gid.png)  
![User login success](./screenshots/10-user-login-success.png)  
![Verify Home Directory](./screenshots/09-verify-user-home-dir.png)

Attempts to elevate privileges using `sudo` or switch users using `su` were intentionally denied. This confirms that only explicitly authorised accounts can perform administrative actions, enforcing least-privilege access.

![Verify sudo access](./screenshots/10-verify-sudo-access.png)

---

### Commands Used
```bash
usermod -l <new-username> <old-username>
groupmod -n <new-groupname> <old-groupname>
ls -ld /home/<username>
useradd -m -s /bin/bash <username>
getent passwd <username>
id <username>
sudo -l -U <username>
```

### Reflection
In this task I learned that managing user accounts in Linux often requires multiple steps to keep usernames, groups, and home directories consistent. Creating and validating role-based users reinforced the importance of verifying access and permissions rather than relying on defaults. I’m becoming more comfortable with the process, but I’ll need additional practice with this workflow to make it feel more natural and repeatable.

---