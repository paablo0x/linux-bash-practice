# Bash Commands Practice

## Navigation

- `ls`, `cd`, `pwd`
- `tree` to view folder structures
- `ls -la` to show hidden files and detailed information
- `cd ..` to go back one directory
- `cd ~` to go to the home directory
- `cd -` to go back to the previous directory

## Files and Directories

- `mkdir folder` to create a directory
- `touch file.txt` to create an empty file
- `cp file.txt backup.txt` to copy a file
- `mv file.txt folder/` to move a file
- `mv old.txt new.txt` to rename a file
- `rm file.txt` to remove a file
- `rm -r folder` to remove a directory and its contents

## Permissions

- `chmod 755 file`
- `chown user:group file`
- `ls -l` to check permissions
- `chmod +x script.sh` to make a script executable
- `chmod -x script.sh` to remove execute permission

## Searching

- `find . -name "*.txt"`
- `grep "text" file.txt`
- `grep -r "text" .` to search recursively
- `which command` to find where a command is located
- `locate filename` to search for files

## Viewing Files

- `cat file.txt` to print the whole file
- `less file.txt` to read a file page by page
- `head file.txt` to show the beginning of a file
- `tail file.txt` to show the end of a file
- `tail -f logfile.log` to follow a log file as it changes

## Pipes and Redirects

- `ls -l | grep ".sh"`
- `echo "Hello" > file.txt`
- `cat file.txt >> log.txt`
- `command > output.txt` to save output to a file
- `command 2> error.txt` to save errors to a file
- `command > output.txt 2>&1` to save normal output and errors
- `command1 | command2` to send the output of one command into another

## Text Processing

- `sort file.txt` to sort lines
- `uniq file.txt` to remove repeated lines
- `wc -l file.txt` to count lines
- `cut -d ":" -f1 /etc/passwd` to extract a field
- `tr 'a-z' 'A-Z'` to change lowercase to uppercase

## Processes

- `ps` to show running processes
- `ps aux` to show more information about running processes
- `top` to monitor processes
- `kill PID` to stop a process
- `pkill process_name` to kill processes by name
- `jobs` to show jobs running in the current shell
- `bg` to send a job to the background
- `fg` to bring a background job back

## Networking

- `ip addr` to show network interfaces and IP addresses
- `ip route` to show the routing table
- `ping 8.8.8.8` to test connectivity
- `ss -tuln` to show listening TCP/UDP ports
- `curl https://example.com` to make an HTTP request
- `wget https://example.com/file` to download a file
- `dig example.com` to query DNS
- `hostname -I` to show the system's IP address

## System Information

- `uname -a` to show kernel and system information
- `hostname` to show the hostname
- `whoami` to show the current user
- `id` to show user and group information
- `uptime` to show how long the system has been running
- `free -h` to show memory usage
- `df -h` to show disk usage
- `du -sh folder/` to show the size of a directory

## Archives

- `tar -cf archive.tar folder/` to create a tar archive
- `tar -xf archive.tar` to extract a tar archive
- `tar -czf archive.tar.gz folder/` to create a compressed archive
- `tar -xzf archive.tar.gz` to extract a compressed archive

## Package Management

Fedora uses `dnf` for package management.

- `sudo dnf install package` to install a package
- `sudo dnf remove package` to remove a package
- `sudo dnf update` to update packages
- `dnf search package` to search for packages
- `dnf info package` to show package information
- `rpm -qa` to list installed RPM packages

## Bash Basics

- `echo "Hello"` to print text
- `history` to show command history
- `clear` to clear the terminal
- `man command` to read the manual for a command
- `command --help` to show basic help
- `$?` to check the exit status of the previous command
- `command1 && command2` to run the second command only if the first succeeds
- `command1 || command2` to run the second command if the first fails
