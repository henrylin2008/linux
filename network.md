* **sudo netstat -ntlp**: check listenting  program network ports 
* **ip -4 addr**: ipv4 address/es
* **netstat -a**: listening all listening ports, including TCP/UDP
* **netstat -at**: all/active TCP ports
* **netstat -l**: all listensing ports
* **netstat -u**: all UDP ports
* **netstat -tln**: listening to TCP ports and display in numeric
	* **-t**: TCP ports
	* **-l**: listening
	* **-n**: numeric 
	* **-s**: statistics 
	* **-p**: program
	* **-r**: route option/routing table 
* **sudo netstat -anp | grep "sshd"**: search for "sshd" and identify the port it is using 
	* **grep ":22"**: search by port 
* **sudo netstat -i**: display a table of the network interfaces 
* **sudo netstat -g**: list the multicast group membership of sockets on each interface 

* **curl -o "File Name"  URL**: store the response from curl into a file 
* **curl -I url**: getting the header
* **curl --help**: all the curl options
* **curl --header "header name"**: send header with the requst: 
	* ex: curl --header "Content-type:application/json" -X POST -d param1=x url"