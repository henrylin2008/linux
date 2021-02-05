### Linux commands:
* **find . -name a.txt**: search current directory and sub-directory with name of a.txt
* **find . -iname A.txt**: search a.txt in current/subdirectory and ignore the (upper/lower) case
* **find . -type d -name a**: find directory named a 
	* **-type d**: directory type 
* **find . -type f**: find all the files including sub-directory (no direcotry)
* **find . -type f -name "test.txt"**: find a file named "test.txt" in current and sub-directories 
	* **-name "test<b>*</b>"** : any file starts with test, and ending with anything 
		* ex: test_1.txt, text_2.txt
	* **-iname**: case insensitive on the name 	

* **find . -type f -mmin -10**: any file was modified in less than 10 minutes ago
* **find . -type f -mmin +10**: any file was modified in more than 10 minutes ago
* **find . -type f -mmin +1 -mmin -5**: any file was modified more than 1 minute ago and  less than 5 minutes ago 
* **find . -type f -mtime -20**: any file was modified in less than 20 days ago 
	* **-mtime**: modified days 
	* **-mtime +20**: more than 20 days ago 
	* **-amin**: access minutes
	* **-atime**: access days
	* **-cmin**: change minutes
	* **-ctime**: change days 

* **find . -size +5M**: find any file more than 5 megabytes
	* **5k**: 5 kilobyte
	* **5G**: 5 Gigabyte 

* **find . -empty**: find all file that is empty 
* **find . -perm 777**: find all files and direcotry with permission 777 

* **find dir1 -exec chown hlin:gp1 {} +**: change user (hlin) and group (gp1) of current directory and subdirectory 
	* **-exec**: execute
	* **chown**: change owner 
	* **{}**: place holder
	* **+** or **\;**: end of the command 
* **find dir1 -type d -exec chmod 775 {} +**: change the permissoin of all directory within dir1 to 775 
* **find dir1 -type f -exec chmod 664 {} +**: change the permission of all files within dir1 to 664
* **find . type f -name "<b>*</b>.jpg" -maxdepth 1**: find all the file with extension .jpg in current directory 