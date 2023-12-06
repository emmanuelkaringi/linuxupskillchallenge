This Journal contains Day 3 (Power Trip), Day 4 (Install & Config files) and Day 5 (Command line basics)

# Day 3 - Power Trip!

- Login with root - `sudo su` / `sudo -i`
- Reboot `sudo reboot`
- Check logs ()- `less /var/log/auth.log`
- Filter to chexk all occurences of 'sudo' - `grep "sudo" /var/log/auth.log`
- Get the hostname - `hostnamectl`
- Set / change the hostname of the computer - `sudo hostnamectl set-hostname somename`
- Check the current system clock time - `timedatectl`
- Set local time of the system clock directly - `sudo timedatectl set-time yyyy-mm-dd hh:mm:ss`
List available timezones - `timedatectl list-timezones`
- Set / change timezone - `sudo timedatectl set-timezone timezone`
- Enable Network Time Protocol(NTP) synchronization - `timedatectl set-ntp on`

# Day 4 - Install & Config files

- Search application - `apt search "application name"`
The package name is the first name before the OS version e.g: mc/focal 3:4.8.24-2ubuntu1 amd64. The package name is `mc`.
- Install packege - `sudo apt install mc`
- Access Configuration file - `less /etc/ssh/sshd_config`

# Day 5 - Command line basics

- Paginate texts appearing on the terminal - `more filelocation or name` `more /var/log/auth.log` or `less`
- Check command history - `history`, `history 5/8/10 etc`, ``
- To repeat a command - `!number of command(position)`
- File that stores the commands history - `less ~/.bash_history`
