**Linux** is an operating system — just like Windows and Mac , An **Operating System (OS)** is software that manages hardware and software resources on a computer or device. It acts as an interface between the user and the computer hardware..
It's open source, very lightweight, and mostly used on servers.
In Linux, you interact a lot using commands (via Terminal / Shell / Bash).
Everything is a file or folder in Linux — even devices are treated as fi*les.

**BASIC COMMANDS:** 
pwd # Present working directory  
cd # Change to the current directory  
ls # List files and directories  
mkdir <folder_name> # Create a new directory  
rmdir <folder_name> # Remove an empty directory  
vi <file_name> # Create a file and edit it  
cp # Copy files or directories  
mv # Move or rename files  
rm <file_name> # Remove a file  
rm -rf <folder_name> # Remove a directory and its contents  
chmod 755 <file_name> # Change file permissions  
kill # Kill a process by its PID  
df -h # Display disk space usage  
curl # Transfer data from or to a server  
ssh @<remote_server> # Connect to a remote server via SSH  
sudo # Run a command with superuser privileges  
ifconfig # Display network interface configuration  
ping <ip_address> # Ping a host to check connectivity  
telnet # Check the connection to a specific port  
scp <file_name> @<remote_server>: # Securely copy a file to a remote server  
cat /etc/os-release # View the OS version  
uname -r # Display kernel version  
systemctl --type=service | grep # Check for a specific service  
systemctl stop/start/disable # Start / Stop / Disable a service  
crontab -e # Edit the crontab for scheduling tasks  
crontab -l # View current cron jobs  
lsblk # List block devices (hard drives, SSDs, partitions)  
