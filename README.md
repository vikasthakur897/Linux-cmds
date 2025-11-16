# Linux Commands

## 1. System Information Commands 

```bash
uname -a           # Full system information
hostname           # Show hostname
hostnamectl        # View/change hostname
uptime             # Show system uptime
arch               # Show system architecture
whoami             # Current logged-in user
who                # List logged-in users
w                  # Show who is logged in and what they are doing
id                 # User and group information
lsb_release -a     # Linux distribution info

```

## 2. Files & Directories

```bash
ls                 # List files
ls -l              # Long list
ls -a              # Show hidden files
cd /path           # Change directory
pwd                # Print working directory
mkdir folder       # Make directory
rmdir folder       # Remove empty directory
rm file            # Remove file
rm -r folder       # Remove directory recursively
cp src dest        # Copy file
cp -r src dest     # Copy folder
mv src dest        # Move/rename
touch file         # Create empty file
cat file           # View file
tac file           # View file reverse
nl file            # Show line numbers
file filename      # Type of file

```

## 3. File Content & Search

```bash
head file          # First 10 lines
tail file          # Last 10 lines
less file          # Scroll view
more file          # Page by page view
grep "text" file   # Search text
grep -r text dir   # Recursive search
wc file            # Word/line count
wc -l file         # Line count
sort file          # Sort lines
uniq               # Remove duplicates
diff file1 file2   # Compare files

```

## 4. Permissions & Ownership

```bash
chmod 755 file                    # Change permissions
chmod u+rwx file                  # Add permission
chown user file                   # Change owner
chown user:group file             # Change owner & group
chgrp group file                  # Change group
umask                             # View mask
stat file                         # Detailed info

```

## 5. Compression & Archiving

```bash
tar -cvf file.tar dir/            # Create tar
tar -xvf file.tar                 # Extract tar
tar -czvf file.tar.gz dir/        # Create tar.gz
tar -xzvf file.tar.gz             # Extract tar.gz
gzip file                         # Compress
gunzip file.gz                    # Decompress
zip -r file.zip folder            # Create zip
unzip file.zip                    # Extract zip

```

## 6. User & Group Management

```bash
useradd username
passwd username
userdel username
groupadd groupname
groupdel groupname
usermod -aG group user
id user
su user
sudo command

```

## 7. Process Management

```bash
ps                    # List processes
ps aux                # Detailed processes
top                   # Real-time monitoring
htop                  # Enhanced top
kill PID              # Kill process
killall name          # Kill by name
jobs                  # Background jobs
fg %1                 # Bring job to foreground
bg %1                 # Move job to background

```

## 8. Networking Commands

```bash
ifconfig              # Show IP & network (older)
ip a                  # Show IP (modern)
ip route              # Routing table
ping google.com       # Check connectivity
curl URL              # Fetch URL
wget URL              # Download file
netstat -tulnp        # Active ports
ss -tulnp             # Replacement for netstat
nslookup domain       # DNS lookup
traceroute host       # Route path
scp file user@host:/  # Secure copy
ssh user@host         # Connect via SSH

```

## 9. Disk & Filesystem

```bash
df -h                 # Disk usage
du -sh folder         # Folder size
mount                 # Show mounted drives
mount /dev/sdX /mnt   # Mount
umount /mnt           # Unmount
fdisk -l              # List partitions
lsblk                 # Block devices
blkid                 # Identify devices
fsck /dev/sdX         # Check filesystem

```

## 10. Package Management (Ubuntu/Debian)

```bash
apt update            # Update repo
apt upgrade           # Upgrade packages
apt install pkg       # Install package
apt remove pkg        # Remove package
apt purge pkg         # Remove config also
apt search name       # Search package

```

## 11. Package Management (CentOS/RHEL)

```bash
yum install pkg
yum remove pkg
yum update
dnf install pkg
dnf remove pkg

```

## 12. Bash Scripting Basics

```bash
#!/bin/bash
echo "Hello World"
read name
if [ condition ]; then
for i in {1..10}
while true
function_name() { }
exit 0

```

## 13. System Services (systemd)

```bash
systemctl status service
systemctl start service
systemctl stop service
systemctl restart service
systemctl enable service
systemctl disable service
journalctl -u service

```

## 14. Others (Very Important)

```bash
history        # Show command history
clear          # Clear screen
date           # Show date time
cal            # Calendar
echo           # Print text
env            # Environment variables
export VAR=1   # Set variable
alias ll="ls -l"
unalias ll

```