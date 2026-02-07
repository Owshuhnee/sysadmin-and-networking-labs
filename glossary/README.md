# Glossary (All Labs)

This glossary defines common words, commands, and concepts used across my System Administration labs.

---

## Virtualisation

- **Host (Host OS):** The physical computer and operating system running the virtualisation software (e.g., Windows 11).
- **Guest (Guest OS):** The operating system running inside a virtual machine (e.g., Ubuntu Server).
- **Hypervisor:** Software that creates and manages virtual machines (e.g., VirtualBox, Hyper-V).
- **Virtual Machine (VM):** A software-based computer that runs its own OS and applications.
- **Snapshot:** A saved state of a VM that allows rollback to a previous point in time.
- **NAT (Network Address Translation):** A networking mode where the VM can access the internet through the host, but inbound access is blocked by default.
- **Bridged Networking:** A networking mode where the VM appears as a separate device on the local network.
- **Isolation:** Separation between host and guest systems to prevent direct interference.

---

## Authentication & Identity

- **Authentication:** Verifying who a user is (usually via username and password).
- **Login shell:** The shell started when a user logs in (e.g., `/bin/bash`).
- **Non-login shell:** A shell started without full login initialization.
- **Environment:** User-specific settings loaded at login, such as variables and profile files.
- **PATH:** An environment variable that defines where the system looks for executable commands.

---

## Users and Groups

- **User:** An account that can log in and run commands.
- **Group:** A collection of users used to manage permissions.
- **Primary group:** The default group assigned to a user at creation.
- **Supplementary group:** Additional groups a user belongs to.
- **UID (User ID):** A unique numeric identifier for a user.
- **GID (Group ID):** A unique numeric identifier for a group.
- **System user:** A non-login account used by services and applications.
- **RBAC (Role-Based Access Control):** Managing access based on roles (groups) instead of individual users.
- **Least privilege:** Granting users only the access required to perform their tasks.

---

## Permissions

- **Owner / Group / Others:** The three permission classes for files and directories.
- **Read (r):** Permission to view file contents or list directory contents.
- **Write (w):** Permission to modify a file or create/delete files in a directory.
- **Execute (x):** Permission to run a file or traverse a directory.
- **chmod:** Command used to change file or directory permissions.
- **chown:** Command used to change file owner and/or group.
- **Numeric (octal) permissions:** A numeric representation of permissions (e.g., `755`, `770`).
- **Special permissions:** Extra permission bits such as setuid, setgid, and sticky bit.
- **setgid:** Causes new files created in a directory to inherit the directory’s group.
- **2770:** Owner and group have full access, others have none, and setgid is enabled.
- **2775:** Same as 2770, but allows others to traverse the directory.
- **Sticky bit:** Prevents users from deleting files they don’t own in a shared directory.

---

## Sudo & Privilege Escalation

- **sudo:** Allows a permitted user to run commands with elevated (root) privileges.
- **sudoers:** Configuration rules that define who can run which commands via sudo.
- **/etc/sudoers:** The main sudo configuration file.
- **/etc/sudoers.d/:** Directory for modular and user-specific sudo rules.
- **visudo:** A safe editor that validates sudo rules before saving.
- **sudo -l:** Lists the commands a user is allowed to run with sudo.
- **Privilege escalation:** Gaining higher permissions than a normal user session.

---

## Filesystem & Directories

- **/home:** Contains user home directories.
- **/etc:** Stores system-wide configuration files.
- **/srv:** Intended location for service-related data.
- **/var:** Variable data such as logs and caches.
- **/root:** Home directory for the root user.
- **Home directory:** A user’s personal working directory.

---

## Configuration Files

- **Configuration file:** A text file that controls how a system or service behaves.
- **sudoers file:** Defines sudo access rules.
- **Modular configuration:** Splitting configuration into smaller files for easier management.
- **Syntax validation:** Checking configuration files for errors before applying them.

---

## Verification & Validation

- **Verification:** Checking that a command or change produced the expected result.
- **Validation:** Ensuring a configuration is correct and safe before use.
- **visudo -c:** Validates sudo configuration files for syntax errors.
- **id:** Displays a user’s UID, GID, and group memberships.
- **ls -ld:** Shows directory ownership and permissions.
- **getent:** Queries system databases such as users and groups.

---

## Command Concepts

- **Flag:** An option that modifies a command’s behavior (e.g., `-a`, `-G`, `-m`).
- **Argument:** A value passed to a command (e.g., a username or directory).
- **Dash (-):** Indicates command options or flags.
- **Login environment (-):** Loads a full user environment when switching users.

---

## Security Concepts

- **Attack surface:** The total number of ways a system can be attacked.
- **Misconfiguration:** Incorrect settings that weaken security.
- **Defense in depth:** Using multiple layers of security controls.
- **Audit:** Reviewing permissions and access to ensure compliance.

---

## File Access Concepts

- **Traverse:** The ability to enter or pass through a directory (execute permission on a directory).
- **Inheritance:** When permissions or ownership are passed down to new files.
- **Access control:** Restricting who can read, write, or execute files.

---
