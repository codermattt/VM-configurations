# Manual Setup on VirtualBox (Ubuntu & CentOs)
Below I will explain the steps I took to manually create virtual machines

## Steps:
1. Enable virtualization settings in BIOS of my windows machine (VTX, secure virtual machine, Virtualization)
2. Disable other windows virtualization settings(Microsoft HyperV, Windows hypervisor platform, Windows subsystem for linux, Docker Desktop, Virtual Machine Platform)
   * restart machine after
3. Creating a new VM instance in VirtualBox (choosing OS type, name, and base memory).
   - Linux
     - Version: Red Hat 64-bit for Centos OR
     - Ubuntu 22.04 (64-bit)
   - Hard-disk setttings automatically allocates the size based off the OS
   - RAM = 2048 mb (2GB or more)
   - Download the Centos Stream 9 ISO, then attach in Settings/Storage as CD/DVD  OR
   - Download the Ubuntu 22 Server ISO, then attach in Settings/Storage as CD/DVD
   3.1  Configuring networking as NAT, and enabling network adapter, for internet and SSH access.
   3.2  Installing the OS manually, including partitioning, setting up users, and updating packages.
   3.3 Install OS, Boot the VM with the ISO mounted, follow on-screen screen instructions for set-up of:
       - User and password
       - Hostname
       - Partitions (default works in most cases)
       - Skip or enable updates
   3.4 After installation, start vm's then get ip adresses of machines with hostnames to ssh into (using Git Bash for e.g)
4. install openssh server on terminal
5. log into VM with - ssh username@ip-address

# notes
Above is a brief run-down of the process I took to manually create my Ubuntu and CentOS Virtual Machines. It helped me a lot, 
in understanding the rest of the things I learned in my Devops journey





    
