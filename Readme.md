# Vagrant OEL Sandbox

## Setup
1. Install Vagrant on OS from https://www.vagrantup.com/downloads.html
2. Download Vagrant box
  ```console
  vagrant box add --name oel7u6 https://yum.oracle.com/boxes/oraclelinux/latest/ol7-latest.box
  ```
  > (Box images are stored in ~/.vagrant.d/boxes - Mac OSX)
3. Initialize Vagrant Box
  ```console
  vagrant init oel7u6
  ```
  > Vagrantfile template is created
4. Edit Vagrantfile
  ```console
  vim Vagrantfile
  ```
5. Run the VM
  ```console
  vagrant up
  ```
6. Connect to VM
  ```console
  vagrant ssh
  ```
7. List available boxes
  ```console
  vagrant box list
  ```
8. List running VMs
  ```console
  vagrant global-status
  ```
9. Stop the VM
  ```console
  vagrant halt oel7-sandbox
  ```
10. Delete the VM
  ```console
  vagrant destroy oel7-sandbox
  ```

## Vagrant Cheatsheet and Tips
* Create vagrant box (vm template) from a running VM:
```console
vagrant package --base my-virtual-machine
```

## Next Steps
* Change network interface to public (bridge)
* Add a second network interface with private network
* Configure disk size
* Create more than one VM

## Notes
https://github.com/oracle/vagrant-boxes

https://yum.oracle.com/boxes

