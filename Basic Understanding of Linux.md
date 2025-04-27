**Linux** is an operating system — just like Windows and Mac , An **Operating System (OS)** is software that manages hardware and software resources on a computer or device. It acts as an interface between the user and the computer hardware..
It's open source, very lightweight, and mostly used on servers.
In Linux, you interact a lot using commands (via Terminal / Shell / Bash).
Everything is a file or folder in Linux — even devices are treated as fi*les.

**BASIC COMMANDS:** 
pwd                  # Present working directory
cd                   # Change to the current directory
ls                   # List files and directories
mkdir <folder_name>  # Create a new directory
rmdir <folder_name>  # Remove an empty directory
vi <file_name>       #create a file and can edit it
cp <source> <destination>  # Copy files or directories
mv <source> <destination>  # Move or rename files
rm <file_name>       # Remove a file
rm -rf <folder_name>  # Remove a directory and its contents
chmod 755 <file_name>  # Change file permissions
kill <pid>           # Kill a process by its PID
df -h                # Display disk space usage
curl <url>           # Transfer data from or to a server
ssh <user>@<remote_server>  # Connect to a remote server via SSH
sudo <command>       # Run a command with superuser privileges
ifconfig             # Display network interface configuration
ping <ip_address>    # Ping a host to check connectivity
telnet <hostname or IP> <port> #check the connection to a specific port
scp <file_name> <user>@<remote_server>:<destination>  # Securely copy a file to a remote server
cat /etc/os-release # View the OS version
uname -r #Display kernel version
systemctl --type=service | grep <Service name> #To check any service
systemctl stop/start/disable <Service name> #To start / stop / disable
crontab -e  #This is used to edit the crontab (cron table) file for scheduling tasks in Linux. Cron is a time-based job scheduler that allows you to run commands , To view current cron jobs use crontab -l
lsblk #this stands for list block devices. In Linux, block devices are physical storage devices like hard drives, SSDs, or even partitions on those drives
