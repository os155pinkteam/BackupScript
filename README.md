BackupScript
============

PinkTeamProject
Title: Backup Script

Problem: You have a computer with multiple users and you want to backup all the files and directories created an hour ago by user os155.
Use tar to backup files. Schedule this job every 5 minutes.


Since this Backup operations must be scheduled every 5 minutes, We must have a command to perform this tasks.

command : crontab -e
(This command will be able to enter into a crontab file and let you edit/issue specific schedule of jobs you want to perform)

At the bottom part of the editor, you will be able to view these:

# m h dom mon dow command
where it corresponds to minutes(0-59), hours(0-23), day of month(1-31), month field(1-12) and day of week(0-6) respectively.
and command you want to execute.

This is now the code:


5 * * * * /location1/location2/pinkteamscript

Note:Make sure that you specify where is the locations of your script you want to run and "pinkteamscript" must be in executable mode e.g (chmod +x pinkteamscript)
