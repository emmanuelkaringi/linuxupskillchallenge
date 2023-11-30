# Day 1 - Get to know your server, Basic navigation

### RTFM (Reading the manual is the first thing)
- `man <command>` - Get the manual of a command.
- `tldr <command>` - Shows a less daunting info about the command.
- `help command` - Display information about a command.
- `type command` - Check if a command is builtin.
- `info` - Reads the documentation stored in info format.

### Got to run the following commands:
1. `uname - a` - Prints the system information.
2. `uptime` - Shows how long the system has been running.
3. `whoami`/ `id -un` - Prints the username of the user currently logged in.
4. `lscpu` - Displays information about the CPU Architecture.
5. `lsblk` - Lists block devices.
6. `lspci` - Lists all PCI devices.
7. `lsusb` - Lists USB devices. (Didn't run in my server, ran on my local system).
8. `free -h` / `vmstat` - Checks the amount of memory used in the system.
9. `top` - Displays the processes and the consumption of resources. (An interactive prettier version is `htop` but needs to be installed).
10. `df -h` - Displays disk usage.
11. `du -h` - Displays the size of your folders.
12. `ifconfig` / `ip address` - Displays your network interfaces and their IP addresses.
13. `nestat -i` / `ifstat` - Displays bandwidth usage.

## Basic navigation
14. `hier` - Description of the file system hierarchy.
15. `cd` - Change directory.
16. `mkdir <name>` - Make / create a new directory/folder.
17. `touch <filename.extension>` - Create a new file.
18. `rm <filename>` - Delete a file.
19. `rm -r <directory name>` - Remove a non empty directory.
18. `rmdir` - Remove a directory.
19. `mv <filename> <newfilename/directoryname>` - Used to move a file or directory to a new location or rename an existing file.
