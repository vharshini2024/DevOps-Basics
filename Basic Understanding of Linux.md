**Linux** is an operating system — just like Windows and Mac , An **Operating System (OS)** is software that manages hardware and software resources on a computer or device. It acts as an interface between the user and the computer hardware..
It's open source, very lightweight, and mostly used on servers.
In Linux, you interact a lot using commands (via Terminal / Shell / Bash).
Everything is a file or folder in Linux — even devices are treated as files.

**BASIC COMMANDS:** 



# Essential Linux Commands for DevOps Engineers

## Basic Navigation
- `pwd` → Present working directory
- `cd <directory>` → Change directory
- `ls` → List files and directories
- `ls -l` → List with detailed permissions
- `mkdir <folder_name>` → Create a new directory
- `rmdir <folder_name>` → Remove an empty directory

## File Management
- `vi <file_name>` → Create or edit a file using vi editor
- `cp <source> <destination>` → Copy files or directories
- `mv <source> <destination>` → Move or rename files
- `rm <file_name>` → Remove a file
- `rm -rf <folder_name>` → Force remove directory and contents
- `chmod 755 <file_name>` → Change file permissions

## Process Management
- `ps aux` → View running processes
- `kill <PID>` → Kill a process by PID
- `top` → Live view of running processes and resource usage
- `htop` → (If installed) Better visual version of top

## Disk and System Info
- `df -h` → Display disk space usage
- `lsblk` → List block devices (drives, partitions)
- `uname -r` → Display kernel version
- `cat /etc/os-release` → View OS version and details

## Networking
- `ifconfig` → View network interfaces and IP addresses
- `ping <ip_address>` → Test network connectivity
- `telnet <ip_address> <port>` → Check if a port is open
- `curl <URL>` → Transfer data from or to a server
- `ssh user@remote_server` → SSH into a remote server
- `scp <file> user@remote_server:/path/` → Securely copy files to/from remote

## Services and Scheduling
- `systemctl --type=service | grep <service_name>` → Check a specific service
- `systemctl start/stop/disable <service>` → Manage a service
- `crontab -e` → Edit user cron jobs
- `crontab -l` → List current cron jobs

## Superuser Commands
- `sudo <command>` → Execute a command as superuser (admin)

  # Linux Slightly Advanced Topics

---

## 1. Users and Groups

- In Linux, **users** are like people who use the system.
- **Groups** are like a team of users, sharing permissions.

### Commands:

| Purpose | Command |
|:---|:---|
| Create a new user | `sudo adduser <username>` |
| Create a new group | `sudo groupadd <groupname>` |
| Add user to a group | `sudo usermod -aG <groupname> <username>` |
| List all users | `cat /etc/passwd` |
| List all groups | `cat /etc/group` |
| Switch user | `su - <username>` |

### Example:
```bash
sudo adduser harshini
sudo groupadd devops_team
sudo usermod -aG devops_team harshini
su - harshini



# `chmod` and `chown` Commands 

---

## `chmod` (Change File Permissions)

**`chmod`** is used to change the permissions (who can read, write, or execute) of a file or directory.

### Permission Types:
- **r** = read
- **w** = write
- **x** = execute (run)

---

### Numeric Permission Values:
| Permission | Value |
|:---|:---|
| Read | 4 |
| Write | 2 |
| Execute | 1 |

---

### Combining Permissions:
| Action | Number | Description |
|:---|:---|:---|
| Read-only | 4 | Only read is allowed |
| Write-only | 2 | Only write is allowed |
| Execute-only | 1 | Only execute is allowed |
| Read + Write | 6 | Read + Write allowed |
| Read + Execute | 5 | Read + Execute allowed |
| Full access (Read + Write + Execute) | 7 | Full access allowed |

---

### Example Commands:

- Give full permission to **owner** and **read-only** to others:
  ```bash
  chmod 744 file.txt
  ```

- Give **read + write** to **owner + group**, and **read** to others:
  ```bash
  chmod 664 file.txt
  ```

---

## `chown` (Change File Owner)

**`chown`** is used to change the ownership of a file or directory (who owns the file and which group it belongs to).

### Example Commands:

- Change owner of file to `harshini`:
  ```bash
  sudo chown harshini file.txt
  ```

- Change owner and group of file to `harshini` and `devops_team`:
  ```bash
  sudo chown harshini:devops_team file.txt
  ```

---

## Quick Reference Summary:

| Action | Command Format |
|:---|:---|
| Change file permissions | `chmod 755 file.txt` |
| Change file owner | `chown user file.txt` |
| Change file owner and group | `chown user:group file.txt` |

---

### Visual Summary:

#### File Permissions (`chmod`):

```
User | Group | Others
  7     5      5
(rwx) (r-x)  (r-x)
```

**Command:**
```bash
chmod 755 file.txt
```

