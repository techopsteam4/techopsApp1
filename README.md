On the loaded jenkins UI => Manage Jenkins => manage plugins =>  install Thinbackup plugin 
on the backend of the loaded server in /home/ubuntu
creat a directory as mkdir -p /techops/jenkins_backup
sudo chown jenkins:jenkins -p /techops/jenkins_backup for jenkins user to write to the directory 
cd into the directory which is your mount point for backups
On UI manage jenkins  => ThinBackup => settings put backup dir -p /techops/jenkins_backup 
do cron job setting for the time of execution making sure file logs are not backup 
tick 
BACKUP BUILD ARCHIVE 
BACKUP USER CONTENT FOLDER
BACKUP PLUGIN ARCHIVES
MOVE OLD BACKUPS TO ZIP¨FILE
Click on Backup and do an ls on CLI in /techops/jenkins_backup

