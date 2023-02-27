### Could not chdir to home directory /home/user: Permission denied


ls -l /
ls -l /home

sudo chmod +x /home
sudo chmod 750 /home/user
sudo chown -R user:user /home/user
