* **env**: list variables 
* **printenv "Variable Name"**: print environment variable
	* or **$"Variable Name"**
* **export VAR="Variable Name"**: create a temp variable on current running session 
* **nano .bashrc**: create env variable/s on an user profile: 
	* **export "Variable Name"="Information"**: add this command anywhere on th file, typically on the top of the file (save and exit file )
	* **source .bashrc**: update .bashrc file to store new variable 
* cd /etc, **nano environment**: create global environment file
	* **export "Variable Name"="Information"**: add this export command in environment file
	* **source environment**: active newly created environment variable/s 
* **unset "Variable Name"**: remove "variable name" from current running session 
