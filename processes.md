* **top**: list process, monitor the most active processes, updating the display at regular intervals
	* **nN**: perform N updates, then quit
	* **d N**: Update the display every N  seconds. 
	* **p N p M**: Display only the processes with PID N, M, ..., up to 20 processes. 
	* **c** Display the command-line arguments of processes. 
	* **b** Print on standard output noninteractively, without playing screen tricks. top b n1 > outfile saves a quick snapshot to a file. 
* **htop**: (apt install htop)
	* **F9**: SIGNKILL
* **kill** [ options ] [ process_ids ] 
	* **kill KILL [process id]**: if it did not get terminated from kill
	* **killall** [process name]
	* **kill -N PID**: N:signal number 
	* **kill -NAME PID**: name:signal name
	* **kill -STOP PID**: freeze a process 
	* **kill -CONT pid**: continue running the process again 
* **ps**: user process/es run by the root user
	* **ps -ux**: your process 
		* **| grep program**
	* **ps -efww**: all processes with full command lines 
* **free**: memory usage in kilobytes: 
	* **s N** Run continuously and update the display every N  seconds. 
	* **b** Display amounts in bytes. 
	* **m** Display amounts in megabytes. 
	* **t** Add a totals row at the bottom. 
	* **o** Don’t display the “buffers/cache” row. 
* **uptime**: how long the system has been running since the last boot: 
* **timeout [ options ] seconds command...**: sets a time limit for running another program, in seconds. 
 	* **-s signal** Send a signal other than the default (TERM). The choices are the same ones listed by kill -l . 
 	* **-k seconds** If the program doesn’t die after the first signal, wait this many seconds longer and send a deadly KILL signal. 

