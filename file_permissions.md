* **chmod [who][+,-,=][permission(s)] filename**
	* **who**:
		* **u**: user/s
		* **g**: group/s
		* **o**: others, anyone but the user and the group
		* **a**: all: everyone, including user/s and group/s 
	* ex:
		* **chmod a+w** abc.txt: add write permission to all
			* -r**w**-r**w**-r**w**- abc.txt
		* **chmod u+x** abc.txt: 
			* -rw**x**-rw-rw-
* chmod -R ()dir: recursivly changing the files permission inside the directory
	* chmod -R **a+w** a: 
		* drwxr-xr-x --> drwxr**w**xr**w**x