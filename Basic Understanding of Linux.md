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

