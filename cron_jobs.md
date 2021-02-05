# ┌───────────── minute (0 - 59)
# │ ┌───────────── hour (0 - 23)
# │ │ ┌───────────── day of month (1 - 31)
# │ │ │ ┌───────────── month (1 - 12)
# │ │ │ │ ┌───────────── day of week (0 - 6) (Sunday to Saturday;
# │ │ │ │ │                                       7 is also Sunday on some systems)
# │ │ │ │ │
# │ │ │ │ │
# * * * * *  command_to_execute


* **crontab -l**: list of cron jobs
* **crontab -e**: cron job editor, creating cron jobs 

* * * * * echo 'Hello' >> /tmp/test.txt: print 'Hello' to test.txt file every minute 

30 * * * * command: it runs every 30 minutes
0 0 * * 1 command: every Monday at midnight 
0 0 1,15 * * command: midnight at 1st and 15th 
*/10 * * * * command: every 10 minutes 
0 0 */3 * * command: every 3 days 
0 0-5 * * * command: every hour from midnight to 5 AM 
*/30 9-17 * * 1-5 command: Monday-Friday, 9am-5pm, every 30 minutes 