# Vagrant OEL Sandbox

## Setup
1. Install Vagrant on OS from https://www.vagrantup.com/downloads.html
2. Download Vagrant box
  ```bash
  vagrant box add --name oel7u6 https://yum.oracle.com/boxes/oraclelinux/latest/ol7-latest.box
  ```
  (Box files are stored in ~/.vagrant.d/boxes - Mac OSX)
3. Initialize Vagrant Box
  ```bash
  vagrant init oel7u6
  ```
  Vagrantfile template is created
4. Edit Vagrantfile
  ```bash
  vim Vagrantfile
  ```
5. Run the VM
  ```bash
  vagrant up
  ```
6. Connect to VM
  ```bash
  vagrant ssh
  ```
7. List available boxes
  ```bash
  vagrant box list
  ```
8. List running VMs
  ```bash
  vagrant global-status
  ```
9. Stop the VM
  ```bash
  vagrant halt oel7-sandbox
  ```
10. Delete the VM
  ```bash
  vagrant destroy oel7-sandbox
  ```

## Next Steps
* Change network interface to public (bridge)
* Add a second network interface with private network
* Configure disk size
* Create more than one VM

## Notes
https://github.com/oracle/vagrant-boxes
https://yum.oracle.com/boxes

