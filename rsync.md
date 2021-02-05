* **rsync Original/ Destination/**
	* original/destination: can be a remote host: user@ip:~/(dir)
* **rsync -r Original/ Destination/**: recrusively sync directory and subdirectories 
	* **-a**: archive, recrusviely, retain permission, symbolic links
	* **--dry-run**: dry run 
	* **-v --dry-run**: verbose, display what files/directories to be copies over
	* **-z**: compress
	* **-P** or **--progress**: showing progress 
