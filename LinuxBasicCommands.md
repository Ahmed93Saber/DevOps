### Basic Linux Commands Cheat Sheet

#### **1. File and Directory Commands**
- **`ls`**: List files and directories in the current directory
  - `ls -l`: List with detailed information
  - `ls -a`: Show hidden files
- **`cd [directory]`**: Change directory
  - `cd ..`: Go up one directory
  - `cd ~`: Go to home directory
- **`pwd`**: Print working directory (shows the current directory)
- **`mkdir [directory]`**: Create a new directory
- **`rmdir [directory]`**: Remove an empty directory
- **`rm [file]`**: Delete a file
  - `rm -r [directory]`: Delete a directory and its contents
- **`cp [source] [destination]`**: Copy files or directories
- **`mv [source] [destination]`**: Move or rename files or directories
- **`touch [file]`**: Create an empty file or update a file’s timestamp
- **`cat [file]`**: View contents of a file
- **`less [file]`**: View file content one page at a time

#### **2. Permissions and Ownership**
- **`chmod [permissions] [file]`**: Change file permissions
  - `chmod 755 [file]`: Set read, write, execute for owner; read and execute for group and others
- **`chown [owner]:[group] [file]`**: Change file owner and group
  - `sudo chown user:user [file]`: Change owner of a file (requires sudo)

#### **3. System Information**
- **`uname -a`**: Show system information (kernel name, version, etc.)
- **`top`**: Display running processes and system resource usage
- **`df -h`**: Display disk space usage (human-readable format)
- **`du -sh [directory]`**: Display disk usage of a directory
- **`free -h`**: Show memory usage (human-readable format)
- **`uptime`**: Show how long the system has been running
- **`whoami`**: Display the current user

#### **4. Process Management**
- **`ps`**: Display active processes
  - `ps aux`: Show all running processes
- **`kill [PID]`**: Kill a process using its Process ID
  - `kill -9 [PID]`: Forcefully kill a process
- **`pkill [name]`**: Kill processes by name
- **`jobs`**: List background jobs
- **`fg`**: Bring a background job to the foreground

#### **5. Network Commands**
- **`ping [hostname/IP]`**: Send ICMP request to check network connection
- **`ifconfig`**: Show network interfaces and IP address
- **`netstat -tuln`**: Show open ports and listening services
- **`curl [URL]`**: Fetch data from a URL
- **`wget [URL]`**: Download a file from the internet

#### **6. Searching and Finding Files**
- **`find [path] -name [filename]`**: Search for files by name
- **`grep [pattern] [file]`**: Search for a pattern in a file
  - `grep -r [pattern] [directory]`: Recursively search within a directory
- **`locate [filename]`**: Find files by name (uses a prebuilt database)
- **`which [command]`**: Find the path of a command

#### **7. Archiving and Compression**
- **`tar -czvf [archive.tar.gz] [directory]`**: Create a compressed archive
- **`tar -xvzf [archive.tar.gz]`**: Extract a compressed archive
- **`zip [archive.zip] [file1] [file2]`**: Compress files into a zip archive
- **`unzip [archive.zip]`**: Extract a zip archive

#### **8. User Management**
- **`sudo`**: Execute a command as the superuser
- **`adduser [username]`**: Add a new user
- **`passwd [username]`**: Change the password for a user
- **`deluser [username]`**: Remove a user

#### **9. Package Management**
- **`apt update`**: Update the package list (Debian/Ubuntu)
- **`apt upgrade`**: Upgrade all installed packages
- **`apt install [package]`**: Install a new package
- **`apt remove [package]`**: Remove a package
- **`apt search [package]`**: Search for a package

#### **10. Shortcuts and Misc**
- **`Ctrl + C`**: Stop/kill the current process
- **`Ctrl + Z`**: Suspend the current process and send it to the background
- **`Ctrl + D`**: Log out or close the terminal
- **`history`**: Show command history
  - `!n`: Re-execute command number `n` from history

#### **11. File Viewing and Editing**
- **`nano [file]`**: Open a file in the nano text editor
- **`vim [file]`**: Open a file in the vim text editor
- **`head [file]`**: View the first 10 lines of a file
  - `head -n [number] [file]`: View the first `n` lines of a file
- **`tail [file]`**: View the last 10 lines of a file
  - `tail -f [file]`: Continuously monitor a file (useful for logs)

This cheat sheet should cover most of the common tasks you'll perform in a Linux environment!
