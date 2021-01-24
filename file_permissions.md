* **chmod [who][+,-,=][permission(s)]** filename
	* **who**:
		* **u**: user/s
		* **g**: group/s
		* **o**: others, anyone but the user and the group
		* **a**: all: everyone, including user/s and group/s 
	* ex:
		* **chmod a+w** abc.txt: add write permission to all
			* -rw-r--r-- --> -r**w**-r**w**-r**w**- abc.txt
		* **chmod u+x** abc.txt: add write permission to the user
			* -rw**x**-rw-rw-
* **chmod -R** (dir): recursivly changing the files permission inside the directory
	* **chmod -R a+w** a: add write permission to directory a  
		* drwxr-xr-x a --> drwxr**w**xr**w**x a
	* **chmod -R a-w** a: remove write permission from directory a
		* drwxrwxrwx a--> dr**-**xr**-**xr**-**x  a
	* **chmod -R a=w** a: set only write permission on directory a
		* d-**w**--**w**--**w**--
	* **chmod a=wr** abcd.txt
		* -**rw**-**rw**-**rw**- abcd.txt 
	* **chmod +x** abcde.txt: adds excute permission for all
	* chmod **g+w,o-rw,a+x** abcde.txt, mutiple permssion separated by **,**
		* -r**wx**rw**x-**-**x**: abcde.txt