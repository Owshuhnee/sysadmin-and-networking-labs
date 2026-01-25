# Sudo and Sudoers

## `visudo`
### What it does
Safely edits or checks sudo configuration.

### Why it matters
If you break sudo rules, you can lock yourself out of admin access. `visudo` helps prevent that by validating the file.

### Commands used
- `sudo visudo -f /etc/sudoers.d/admins`
- `sudo visudo -c`

### Explain like I'm 5
Sudo rules are like “who is allowed to be the boss”.
`visudo` is the safe tool that checks the rules before saving.

---

## `/etc/sudoers.d/`
### What it is
A folder where you can place separate sudo rule files (cleaner than editing the main `/etc/sudoers` file).

### Your file
- `/etc/sudoers.d/admins`

Typical content might look like:
```conf
%admins ALL=(ALL:ALL) ALL
```

## `chmod 440 (sudoers files)`
### What it does
Sets strict permissions on the sudoers rules file.

Command used
```bash
sudo chmod 440 /etc/sudoers.d/admins
```

### Explain like I'm 5
Only the system should be able to read the rules properly, and nobody should casually edit them.
Why 440:
- Owner: read
- Group: read
- Others: no access