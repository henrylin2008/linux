### Users and Groups: 
* **adduser** (username) 
* **cat** /etc/passwd: all users in the system
* **deluser** (username): remove user and the user directory 
* **passwd** (username): update (username) password
* **passwd**: update current user’s password 
* **addgroup** (group name): create new group
* **usermod -a -G** (group name) (user): add (user) to the (group) 
	* a: append
	* G: group
* **groups** (user): what groups an user is belonged to
* **groups**: what groups current user is belonging to 
* **gpasswd -d** (user) (group): remove (user) from the (group)
* **visudo**: modify group (needs sudoer’s permission) 
	* User privilege specification:  (grant user specific permission) 
		* **(username) ALL=/usr/bin/top, next command**: grant user to specific command/s
		* **ctrl+s** (write to the file), and **ctrl+x** (save the file) 
	* allow members of group sudo to execute any command: (grant group permission) 
		* **(group) ALL=/usr/bin/ls, next command/s**
* **which** (command): find the location of the command
* **delgroup** (group name): delete a group 
