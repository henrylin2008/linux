* **sudo !!**: runs last command with sudo permission
* **Ctrl + K** (in middle of a command): cut everything after the cursor, the rest of command/line
	* **Ctrl + U** (in middle of a command): cut everything before the cursor 
	* **Ctrl + Y**: paste back what was cut (above)  
	* **Ctrl + W**: kill word (by word) backward
* **less +F /var/log/syslog**: view latest log
	* **Ctrl + C**: detach, and allow to scroll up and down on the log file 
	* Shift + F: reattach 
	* Ctrl + C: out of follow mode
	* q: exit 
* **Alt + .**: execute previous success command  
* **reset**: reset the terminal
* **Ctrl+x+e**: Open an editor to run a command 
* leading space: not add command to the history
* **fc**: run last command in an editor
* **ssh -L 3337:127.0.0.1:6379 root@emkc.org -N**: tunnel with ssh (local port 3337 --> remote host's 127.0.0.1 on port 6379)
* **mkdir -p folder/{sub1,sub2}/{sub1,sub2,sub3}**: create folder, 2 subfolders, and 3 sub-subfolders 
* **cat file.txt | tee -a log.txt | cat > /dev/null**: intercept stdout and log to log.txt file 
* **disown -a && exit**: exit terminal but leave all processes running 
	* ex: sleep 123, bg, disown -a && exit; leave sleep 123 process in bg 
	* ps aux | grep sleep: return running process that has sleep 

* uptime: shows the uptime of the system
* wall (message): broadcast a message to all users 
* write (user) /n (message): send a message to one user
* mesg (y/n): enable or disable the ability to recieve messages 
* who: shows all users who are logged into the system 
* free: shows all the system resources being used 
* sort file.txt: sort the file of first letter of each letter/word with ascending order 
* sort -r file.text: sort the file with decedent order 
* shutdown -h "time": shutdowns the machien at a specified time from command line 
	* shutdown -h now
	* shutdown -h +10: shutdown in 10 minutes 
* shutdown -r "time": restart the machine at a specified time 
	* shutdown -r now: restart the machine now 
* whatis (command): gives a brief description of a command 
	* whatis ls 

