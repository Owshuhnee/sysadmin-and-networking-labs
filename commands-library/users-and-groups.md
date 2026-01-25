# Users and Groups

## `groupadd`
### What it does
Creates a new group.

### Commands used
- `sudo groupadd admins`
- `sudo groupadd developers`

### Explain like I'm 5
You’re making a “team”. Later, you can put people into the team.

---

## `getent group`
### What it does
Looks up information about a group (and confirms it exists).

### Commands used
- `getent group admins`
- `getent group developers`

### Explain like I'm 5
“Show me the team and who is in it.”

---

## `useradd`
### What it does
Creates a new user account.

### Flags you used
- `-m` = create a home folder (like `/home/jove-admin`)
- `-s /bin/bash` = set the default shell to Bash

### Commands used
- `sudo useradd -m -s /bin/bash jove-admin`
- `sudo useradd -m -s /bin/bash jove-dev`

### Explain like I'm 5
You’re creating a new person, giving them a room (home folder), and choosing the type of door they use (their shell).

---

## `passwd`
### What it does
Sets or changes a user’s password.

### Commands used
- `sudo passwd jove-admin`
- `sudo passwd jove-dev`

### Explain like I'm 5
You’re setting a secret code so the user can log in.

---

## `usermod -aG`
### What it does
Adds an existing user to an additional group.

### Flags you used
- `-a` = append (don’t remove other group memberships)
- `-G` = specify supplementary groups

### Commands used
- `sudo usermod -aG admins jove-admin`
- `sudo usermod -aG developers jove-dev`

### Explain like I'm 5
You’re putting the person into a team **without kicking them out of their other teams**.

> Important: Leaving out `-a` can accidentally remove other group memberships.

---

## `id`
### What it does
Shows a user’s user ID and which groups they belong to.

### Commands used
- `id jove-admin`
- `id jove-dev`

### Explain like I'm 5
“Show me this person’s ID card and what teams they’re in.”

---

## `gpasswd -d`
### What it does
Removes a user from a group.

### Command used
- `sudo gpasswd -d jove-dev admins`

### Explain like I'm 5
You’re removing someone from a team.
