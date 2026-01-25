# Glossary (All Labs)

This glossary defines common words and ideas used across my labs.

## Virtualisation
- **Host (Host OS):** Your real computer (e.g., Windows 11).
- **Guest (Guest OS):** The OS running inside the VM (e.g., Ubuntu Server).
- **Hypervisor:** Software that runs VMs (e.g., VirtualBox).
- **Snapshot:** A “save point” for a VM you can roll back to.

## Users and Groups
- **User:** An account that can log in and run commands.
- **Group:** A label you can assign to users. Used to control access to files and permissions.
- **Primary group:** The main group a user belongs to.
- **Supplementary group:** Extra groups a user is added to.

## Permissions
- **Owner / Group / Others:** The three permission “buckets” for a file/folder.
- **chmod:** Changes permissions.
- **chown:** Changes owner and/or group.
- **Least privilege:** Give only the minimum access needed.

## Sudo
- **sudo:** Run a command with admin rights (if you’re allowed).
- **sudoers:** The rules file(s) that decide who can use sudo.
- **visudo:** Safe editor/checker for sudo rules.

## Useful folders
- **/srv:** Common place to store data for services (shared folders, web content, etc.).
- **/etc:** System configuration files.
- **/home:** User home folders.