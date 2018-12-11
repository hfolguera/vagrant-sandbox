# Vagrant OEL Sandbox

## Setup
1. Install Vagrant on OS
  - https://www.vagrantup.com/downloads.html
2. Download Vagrant box
  - `vagrant box add --name oel7u6 https://yum.oracle.com/boxes/oraclelinux/latest/ol7-latest.box`
  - (Box files are stored in ~/.vagrant.d/boxes - Mac OSX)
3. Initialize Vagrant Box
  - `vagrant init oel7u6` 
  - Vagrantfile template is created
4. Edit Vagrantfile
  - `vim Vagrantfile`
5. Run the VM
  - `vagrant up`
6. Connect to VM
  - `vagrant ssh`
7. List available boxes
  - `vagrant box list`
8. List running VMs
  - `vagrant global-status`
9. Stop the VM
  - `vagrant halt oel7-sandbox`
10. Delete the VM
  - `vagrant destroy oel7-sandbox`

## Next Steps
* Change network interface to public (bridge)
* Add a second network interface with private network
* Configure disk size
* Create more than one VM

## Notes
https://github.com/oracle/vagrant-boxes
https://yum.oracle.com/boxes

