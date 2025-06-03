# Automated VM Setup Guide
This guide demonstrates the simple automation of a VM setup using Vagrant

# Auto Setup for Centos
The setup was done in a Git Bash terminal
1. mkdir /C/vagrant-vms; cd /C/vagrant-vms
2. mkdir centos
3. mkdir ubuntu
4. cd centos
5. vagrant init eurolinux-vagrant/centos-stream-9 --box-version 9.0.48   (creates a Vagrantfile off the eurolinux-vagrant/centos-stream-9 box, in current directory)
   *It is optional to configure/edit the Vagrantfile with settings for hostname, network, etc, but VM will still boot up.
7. vagrant up  (start up vm)
   *make sure to disable your anti-virus, VPN's, or use other network if using corporate network

   Common commands used: 
   - vagrant status (check which VM's are up, if any)
   - vagrant ssh (log into vm)
   - sudo -i (switch to root user, escalate priviledges)
   - exit (logout of current user)
   - vagrant halt (power off VM)
   - vagrant reload  (reboot machine, applying changes in VagrantFIle
   - vagrant box list  (list all boxes downloaded on local machine)
# Auto setup for Ubuntu
1. cd /C/vagrant-vms/ubuntu
2. vagrant init ubuntu/jammy64   (download box, to create Vagrantfile)
3. vagrant up
   - vagrant global-status  (check all vm's currently running)
4. vagrant ssh
-----------------------------------------------------------------------------------------
Note: we don't need virtualbox to manage vm, we use vagrant (Git Bash) commands, but we can observe vm's on virtualbox
