# Mysql_backup

Mysql backup script for use in cyberpanel with gzip compression
After that It uploads to mega.nz. I've used the recycle bin in mega.nz as It will automatically delete the files after some time.
###########################################################

# Script: mysql_backup.sh

# Description: Backup all MySQL databases separately

# Author: Hirantha Bandara Muramudali

# Date: March 19, 2023

# Updated on March 20,2023

# Usage: ./mysql_backup.sh

###########################################################

This script retrieves the MySQL password from CyberPanel using the cat command and stores it in the mysql_password variable. Then it uses this password to connect to the MySQL server and back up each database separately. Note that you should make sure that the mysql command is in the system's PATH or provide the full path to the command if it's not.

This script uses the mysql command to get the list of databases, and then iterates over the list to backup each database separately. The resulting backup file for each database is saved in the specified backup directory with a filename that includes the database name and the current date and time.
