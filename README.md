# DB Backup-script

Login into the server

By using ssh command
"ssh -i "pemfile" usernaema@ip

Craete a file by using below command
" touch filename.sh"

Make this file executble by running below command
"chmod +x filename.sh

""Write the given script into the server""

Use the crontab by running below command
crontab e

Write the backup time and file name

# Edit this file to introduce tasks to be run by cron.
#
# Each task to run has to be defined through a single line
# indicating with different fields when the task will be run
# and what command to run for the task
#
# To define the time you can provide concrete values for
# minute (m), hour (h), day of month (dom), month (mon),
# and day of week (dow) or use '*' in these fields (for 'any').#
# Notice that tasks will be started based on the cron's system
# daemon's notion of time and timezones.
#
# Output of the crontab jobs (including errors) is sent through
# email to the user the crontab file belongs to (unless redirected).
#
# For example, you can run a backup of all your user accounts
# at 5 a.m every week with:
# 0 5 * * 1 tar -zcf /var/backups/home.tgz /home/
#
# For more information see the manual pages of crontab(5) and cron(8)
#
# m h  dom mon dow   command
  0 0,6,12,18 * * *         /home/ubuntu/filename.sh
 
