## Navigate the Linux File System

- Linux uses the Filesystem Hierarchy Standard (FHS) to organize files and directories.
- The root directory (`/`) is the top-level directory in Linux.
- File paths identify the location of files and directories.
- Absolute paths start from the root directory, while relative paths start from the current directory.
- Common directories:
  - `/home` → user directories
  - `/bin` → executable files
  - `/etc` → configuration files
  - `/tmp` → temporary files
  - `/mnt` → mounted storage devices
- Important navigation commands:
  - `pwd` → display current directory
  - `ls` → list files and directories
  - `cd` → change directories
- Special path symbols:
  - `.` → current directory
  - `..` → parent directory
  - `~` → user’s home directory

---

## Manage File Content in Bash

- `cat` displays the full contents of a file.
- `head` shows the beginning of a file (default 10 lines).
- `tail` shows the end of a file and is useful for log monitoring.
- `less` allows scrolling through file content page by page.
- `grep` searches files for specific text patterns.
- Pipes (`|`) send the output of one command as input to another command.
- `find` searches for files and directories using criteria such as name or modification time.
- File management commands:
  - `touch` → create empty files
  - `rm` → delete files
  - `mkdir` → create directories
  - `rmdir` → remove empty directories
  - `mv` → move or rename files
  - `cp` → copy files
- `nano` is a command-line text editor for creating and editing files.
- Output redirection:
  - `>` overwrites file content
  - `>>` appends content to a file

---

## Authenticate and Authorize Users

- Authentication verifies a user’s identity.
- Authorization determines what resources a user can access.
- Linux permissions are represented with a 10-character string.
- Permission types:
  - `r` → read
  - `w` → write
  - `x` → execute
- Permission categories:
  - User (`u`)
  - Group (`g`)
  - Other (`o`)
- `ls -l` displays file permissions and ownership information.
- `chmod` changes file and directory permissions.
- Principle of least privilege:
  - Users should only have the minimum access necessary.
- `sudo` temporarily grants elevated privileges to authorized users.
- User management commands:
  - `useradd` → create users
  - `usermod` → modify users
  - `userdel` → delete users
- `chown` changes file or directory ownership.

---

## Get Help in Linux

- Linux has a large online community for troubleshooting and learning.
- :contentReference[oaicite:0]{index=0} is a popular Linux Q&A resource.
- `man` displays detailed manuals for commands.
  - Example: `man chmod`
- `apropos` searches command descriptions using keywords.
  - Example: `apropos editor`
- `whatis` provides a short description of a command.
  - Example: `whatis nano`
- Man pages include:
  - command syntax
  - options
  - usage examples
- Built-in help commands are useful for troubleshooting and learning new commands.