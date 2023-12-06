This journal contains Day 6 (Vim Crash Course), Day 7 (Installing Apache), Day 8 (Text Processing)

# Day 6 - Vim Crash Course

- Check Vim version - `vi --version`
- Create file - `vi filname`
- Close without saving - `:q` or `:q!` to force quit.
- Open a file - `vim filename` eg. `vim services` can also be used to create a file if it does not exist.
- Save file - `:w`
- Save as - `:w newfilename`
- Save and close - `:wq`
- Insert mode - `i`
- Get back to normal mode - `esc` button.
- Visual mode - `v`
- Delete entire line - `dd`
- Copy/yank - `y` in visual mode(`v`)
- Copy entire line - `yy`
- Paste - `p`
- Revert or undo - `u`
- Redo - `crtl + R`
- Find a phrase - `/phrase`, `n` to go to the next.
- Find and Replace - `:%s/oldword/newword/gc`

# Day 7 - Installing Apache

- Install Apache - `sudo apt install httpd`
- Check status of the web server or any process - `sudo systemctl status httpd`
- To start webserver - `sudo systemctl start httpd`
- Stop or restart the server - `sudo systemctl stop/restart httpd`
- Configure the web server to start with each system boot - `sudo systemctl enable httpd`. The opposite is `disable`
- Change the default index file - `sudo vim /var/www/html/index.html`
- Check logs - `less /var/log/httpd/access.log`

# Day 8 - Text Processing

- Display message on the screen - `echo "Hello World"`
- Print on the screen the content of a file - `cat filename`
- Print on the screen but in reverse - `tac filename`
- Print the first few lines - `head filename` e.g. `head -5 filename` print first five lines.
- Print the last few lines - `tail filename`
- Word count - `wc -l filename`
- Print only the unique lines - `uniq filename`
- `grep "searchterm" filename`
- Append information - `echo "hello world" filename`
- Pipping