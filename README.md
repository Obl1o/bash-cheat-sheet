<p align="center"><img align="center" src="/images/bcs_logo.webp"</p> 

<br>
<br>
A handy cheat sheet for essential Bash commands, covering file management, process handling, networking, and more. Perfect for beginners and experienced users looking for a quick reference. **Printable PDF available in the "release" section**.
<br>
<br>  
  
## Basic Commands

| Command                 | Description                                                                 |
|-------------------------|-----------------------------------------------------------------------------|
| `pwd`                   | Print working directory                                                     |
| `ls`                    | List directory contents                                                     |
| `cd <directory>`        | Change directory to `<directory>`                                           |
| `touch <file>`          | Create an empty file                                                        |
| `mkdir <dir>`           | Create a new directory                                                      |
| `rm <file>`             | Remove a file                                                               |
| `rmdir <dir>`           | Remove an empty directory                                                   |
| `rm -r <dir>`           | Remove a directory and its contents                                         |
| `cp <source> <dest>`    | Copy files or directories                                                   |
| `mv <source> <dest>`    | Move or rename files or directories                                         |

## File Permissions

| Command                         | Description                                                         |
|---------------------------------|---------------------------------------------------------------------|
| `chmod <permissions> <file>`    | Change file permissions (e.g. `chmod 755 file`)                     |
| `chown <user>:<group> <file>`   | Change file ownership                                               |
| `ls -l`                         | List files with detailed information                                |
| `chmod -R <permissions> <dir>`  | Change permissions recursively for a directory                      |
| `chown -R <user>:<group> <dir>` | Change ownership recursively for a directory                        |

## File Viewing & Editing

| Command                          | Description                                                        |
|----------------------------------|--------------------------------------------------------------------|
| `cat <file>`                     | Display the contents of a file                                     |
| `less <file>`                    | View a file page by page                                           |
| `head <file>`                    | View the first 10 lines of a file                                  |
| `tail <file>`                    | View the last 10 lines of a file                                   |
| `vim <file>`                     | Open a file in the Vim editor                                      |
| `vim +<line> <file>`             | Open a file and jump to a specific line number                     |

## Searching & Finding Files

| Command                          | Description                                                        |
|----------------------------------|--------------------------------------------------------------------|
| `grep <pattern> <file>`          | Search for a pattern in a file                                     |
| `find <path> -name <file>`       | Find a file by name                                                |
| `locate <file>`                  | Locate a file by its name                                          |
| `updatedb`                       | Update the database for `locate`                                   |
| `which <command>`                | Find the location of a command in the system path                  |
| `whereis <command>`              | Find binary, source, and manual pages of a command                 |

## Process Management

| Command                          | Description                                                        |
|----------------------------------|--------------------------------------------------------------------|
| `ps`                             | List processes running on the system                               | 
| `top`                            | Display a real-time list of running processes                      |
| `kill <pid>`                     | Kill a process by its PID                                          |
| `killall <process>`              | Kill all instances of a process                                    |
| `bg`                             | Move a process to the background                                   |
| `fg`                             | Bring a background process to the foreground                       |
| `nice <command>`                 | Start a command with a modified priority                           |
| `renice <priority> <pid>`        | Change the priority of a running process                           |
| `nohup <command> &`              | Run a command in the background and ignore hangups                 |
| `pstree`                         | Display processes in a tree-like format                            |

## Networking

| Command                          | Description                                                        |
|----------------------------------|--------------------------------------------------------------------|
| `ping <host>`                    | Ping a host to check connectivity                                  |
| `curl <url>`                     | Transfer data from or to a server                                  |
| `wget <url>`                     | Download files from the web                                        |
| `ifconfig`                       | Display or configure network interfaces                            |
| `ip a`                           | Display network interfaces (more modern than `ifconfig`)           |
| `ss`                             | Utility to investigate sockets (faster and better than `netstat`)  |
| `traceroute <host>`              | Trace the path packets take to a destination                       |
| `nslookup <domain>`              | Query DNS to find domain information                               |
| `dig <domain>`                   | Perform DNS queries and display the results                        |
| `hostname`                       | Show or set the system's hostname                                  |
| `telnet <host> <port>`           | Test connectivity to a specific port on a remote host              |
| `scp <file> <user>@<host>:<path>`| Copy files securely between hosts via SSH                          |
| `rsync <source> <destination>`   | Synchronize files between local and remote systems                 |

## Disk Usage

| Command                          | Description                                                        |
|----------------------------------|--------------------------------------------------------------------|
| `df`                             | Show disk space usage                                              |
| `du`                             | Show disk usage of files and directories                           |
| `du -sh <dir>`                   | Show the total disk usage of a directory in human-readable format  |
| `mount`                          | Mount a filesystem                                                 |
| `umount <device>`                | Unmount a filesystem                                               |
| `lsblk`                          | List information about block devices                               |
| `fdisk -l`                       | List all partitions and their details                              |
| `parted -l`                      | List partitions in a human-readable format                         |
| `fsck <device>`                  | Check and repair a filesystem                                      |
| `tune2fs -l <device>`            | View information about an ext2/ext3/ext4 filesystem                |

## System Information

| Command                          | Description                                                        |
|----------------------------------|--------------------------------------------------------------------|
| `uname -a`                       | Display system information (kernel, OS, etc.)                      |
| `hostnamectl`                    | Get or set the system hostname                                     |
| `uptime`                         | Show system uptime and load averages                               |
| `who`                            | Show who is logged in                                              |
| `w`                              | Display who is logged in and their activity                        |
| `last`                           | Show the last logins                                               |
| `free`                           | Display memory usage                                               |
| `vmstat`                         | Report virtual memory statistics                                   |
| `lscpu`                          | Display CPU architecture information                               |
| `lsusb`                          | List USB devices                                                   |
| `lspci`                          | List PCI devices                                                   |
| `dmesg`                          | Print the kernel ring buffer                                       |
| `lshw`                           | Display detailed hardware configuration                            |
| `top`                            | Monitor system resources in real-time                              |

## Environment Variables

| Command                          | Description                                                        |
|----------------------------------|--------------------------------------------------------------------|
| `echo $<variable>`               | Print the value of an environment variable                         |
| `export <variable=value>`        | Set an environment variable                                        |
| `unset <variable>`               | Remove an environment variable                                     |
| `env`                            | Display all environment variables                                  |
| `printenv`                       | Print all environment variables                                    |

## File Redirection & Pipes

| Command                          | Description                                                        |
|----------------------------------|--------------------------------------------------------------------|
| `command > <file>`               | Redirect output to a file                                          |
| `command >> <file>`              | Append output to a file                                            |
| `command < <file>`               | Use a file as input to a command                                   |
| `command \| <command>`           | Pipe output from one command to another                            |
| `command 2> <file>`              | Redirect error output to a file                                    |
| `command &> <file>`              | Redirect both stdout and stderr to a file                          |

## Special Characters

| Character                        | Description                                                        |
|----------------------------------|--------------------------------------------------------------------|
| `*`                              | Wildcard, matches zero or more characters                          |
| `?`                              | Matches any single character                                       |
| `[]`                             | Matches any one character within the brackets                      |
| `&`                              | Run a command in the background                                    |
| `\|`                             | Pipe the output of one command to another                          |
| `;`                              | Separate multiple commands on the same line                        |
| `&&`                             | Execute the second command only if the first succeeds              |
| `\|\|`                           | Execute the second command only if the first fails                 |

## Useful Variables

| Variable                        | Description                                                         |
|---------------------------------|---------------------------------------------------------------------|
| `$HOME`                         | Home directory                                                      |
| `$USER`                         | Current user                                                        |
| `$PATH`                         | List of directories to search for executables                       |
| `$PWD`                          | Current working directory                                           |
| `$SHELL`                        | The path to the current shell                                       |

## Other Useful Commands

| Command                          | Description                                                        |
|----------------------------------|--------------------------------------------------------------------|
| `alias <name>='<command>'`       | Create an alias for a command                                      |
| `unalias <name>`                 | Remove an alias                                                    |
| `man <command>`                  | Show the manual page for a command                                 |
| `info <command>`                 | Show detailed documentation for a command                          |
| `crontab -l`                     | List scheduled cron jobs                                           |
| `systemctl <command>`            | Control systemd services (start, stop, restart)                    |
| `service <service> <action>`     | Manage services (start, stop, restart)                             |
| `journalctl`                     | View logs from the systemd journal                                 |

## CONTRIBUTING
If you find errors or want to suggest the addition of a particular command that you deem important, feel free to submit a pull request.
