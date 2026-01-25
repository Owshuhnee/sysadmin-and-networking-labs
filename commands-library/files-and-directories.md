```md
# Files and Directories (Plain English)

## `mkdir -p`
### What it does
Creates a directory (folder). The `-p` flag creates parent folders if needed, and won’t error if the folder already exists.

### Command used
- `sudo mkdir -p /srv/devshare`

### Explain like I'm 5
“Make this folder, and if the bigger folders don’t exist, make those too.”

---

## `chown owner:group`
### What it does
Changes who owns a file/folder and which group it belongs to.

### Command used
- `sudo chown root:developers /srv/devshare`

### Explain like I'm 5
You’re saying:
- The “boss owner” is `root`
- The “team” is `developers`

So developers can be allowed access via permissions.

---

## `chmod 2770`
### What it does
Changes permissions on a folder.

### Command used
- `sudo chmod 2770 /srv/devshare`

### Break it down (plain English)
- `2` = setgid bit (special)
- `7` = owner can read/write/enter
- `7` = group can read/write/enter
- `0` = others get nothing

### Why the leading `2` matters (setgid)
When new files/folders are created inside `/srv/devshare`, they **automatically inherit the folder’s group** (`developers`).

### Explain like I'm 5
This folder is a “team folder”:
- Only the owner + team can use it
- Anyone else is blocked
- Anything created inside stays part of the team automatically
