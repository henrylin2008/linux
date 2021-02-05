* .bash_profile: login shell when opening terminal (on Mac)
	* in .bash_profile: mirror settings of .bash_profile and .bashrc
		* if [ -f ~/.bashrc ]; then
			source ~/.bashrc
		  fi 
* .bashrc: run on non-login shell, ex: (run) bash on terminal
	* customization in .bashrc file: 
		* PS1="custom--> "; reopen terminal or source .bashrc from terminal, the custom--> view will be showing up on the terminal 
		* PS1="\u-> "; export PS1; 
			* terminal display: username -> 
		* Special characters: 
			* **\h**: hostname up to the first 
			* **\n**: newline
			* **\s**: the name of the shell
			* **\t**: the current time time in 24-hour format
			* **\u**: the username of the current user
			* **\w**: the current working directory
			* **\W**: the basename of the current working directory 
		* PS1="\u@\h \W-> "; export PS1;
			* ex: hlin@hlinMac Desktop -> 
		* PS1="$(tput setaf 166)\u@\h \W -> $(tput sgr0)"; export PS1;
			* **tput setaf 166**: set terminal line to color 166/organge (256 color chart)
			* 228: yellow; 71: green 
			* **tput sgr0**: reset formatting at the end of the prompt
			* can be separated into multiple lines: 
				* PS1= "\[$(tput setaf 166)\]\u";	# organge
				* PS1+= "\[$(tput setaf 228)\]@\h ";	# yellow
				* PS1+= "\[$(tput setaf 71)\]\W -> ";	
				* PS1+="\[$(tput sgr0)\]"; 
				* export PS1; 