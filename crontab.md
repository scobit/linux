#### List crontab jobs for all users
for user in $(cut -f1 -d: /etc/passwd); do crontab -u $user -l; done
