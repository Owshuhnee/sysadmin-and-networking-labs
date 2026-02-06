# 🧸 Command Notes (My Toddler Notes)

Simple explanations for Linux commands I’ve used across my SysAdmin labs.  
Written so Future-Me can understand them quickly.

These notes grow as I learn.

---

## Users & Groups

| Command | Explain like I’m 5 |
|-------|--------------------|
| `useradd -m -s /bin/bash <username>` | Make a new person and give them their own room and a proper shell. |
| `usermod -l <new> <old>` | Change this person’s name but keep their stuff. |
| `usermod -aG <group> <user>` | Add this person to a team without removing them from other teams. |
| `id <user>` | Show this person’s ID card and all their teams. |
| `groupadd <group>` | Make a new team. |
| `groupmod -n <new> <old>` | Rename the team without deleting it. |
| `gpasswd -d <user> <group>` | Remove this person from the team. |
| `getent group <group>` | Show this team and who’s in it. |
| `getent passwd` | Show all user accounts on the system. |
| `getent passwd <user>` | Show this person’s account details. |
| `passwd <user>` | Set or change this person’s password. |
| `passwd -l <user>` | Lock this account so they can’t log in. |
| `passwd -u <user>` | Unlock this account so they can log in again. |
| `passwd -S <user>` | Check whether this account is locked or active. |

---

## Navigation & Identity

| Command | Explain like I’m 5 |
|-------|--------------------|
| `whoami` | Who am I right now? |
| `su - <user>` | Log in as this person properly with their settings. |
| `ls -ld` | Who owns this folder and who is allowed inside? |
| `ls -ld /home/<user>` | Who owns this person’s home folder and who can use it? |

---

## Sudo & Admin Powers

| Command | Explain like I’m 5 |
|-------|--------------------|
| `visudo -f /etc/sudoers.d/admins` | Carefully write rules about who is allowed to be the boss. |
| `chmod 440 /etc/sudoers.d/admins` | Only root can read the rules and nobody can change them. |
| `visudo -c` | Check the rules so I don’t break sudo. |
| `sudo -l` | What boss-level commands am I allowed to run? |
| `sudo passwd <user>` | Force-set or change this person’s password. |

---

## Files & Directories

| Command | Explain like I’m 5 |
|-------|--------------------|
| `mkdir <dir>` | Make a new folder. |
| `mkdir <dir1> <dir2> <dir3>` | Make lots of folders at once. |
| `mkdir -p <path>` | Make the folder and any missing parent folders. |
| `chown <owner>:<group> <dir>` | Decide who owns it and which team it belongs to. |
| `chmod 2770 <dir>` | Only owner and team can use it. New files stay with the team. |
| `chmod 2775 <dir>` | Team can fully use it. Others can look but not change. |
| `ls` | What’s here? |
| `ls -l` | Show who can read, write, or run each file. |
| `ls -d */` | Show only folders. |
| `ls -ld */` | Show folder ownership and permissions. |

---

## Permission Bits

| Value | Meaning |
|------|--------|
| `r = 4` | Read (look inside) |
| `w = 2` | Write (change things) |
| `x = 1` | Execute / enter |

---

## Permissions Library (Quick Reference)

| Mode | Explain like I’m 5 |
|-----|--------------------|
| `2770` | Owner and team can read, write, and enter. Others are blocked. New files stay with the team. |
| `2775` | Owner and team can fully use it. Others can look and enter only. |
| `111` | You can enter or run it, but can’t see or change anything. |
| `555` | Everyone can look and enter, but nobody can change anything. |

---

## Misc Commands

| Command | Explain like I’m 5 |
|-------|--------------------|
| `sudo shutdown now` | Turn the computer off right now. |
| `clear` / `Ctrl + L` | Clean the screen so it’s easier to read. |

---
