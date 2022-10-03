# vagrant_vm_windows10
Create VirtualBox VM in Windows 10 by using Vagrant

### Tools download & preparation:
- cmder : Portable console emulator for Windows 
    (https://cmder.app/)
- VirtualBox: Oracle VirtualBox 6.1.38 platform packages 
    (https://download.virtualbox.org/virtualbox/6.1.38/VirtualBox-6.1.38-153438-Win.exe)
- Vagrant: HashiCorp Vagrant 2.3.1 
    (https://releases.hashicorp.com/vagrant/2.3.1/vagrant_2.3.1_windows_amd64.msi)

### Install procedures:
- Install above pre-downloaded windows package.
- VirtualBox & Vagrant installation needs the local Windows administrator privilege.

### open cmder console & type following commands
  ```
  - mkdir vagrant_ubuntu
  - cd vagrant_ubuntu
  ```
  #### download ubuntu 20.04 box image file
  ```
  - vagrant.exe box add generic/ubuntu2004
  - vagrant.exe box list
  generic/ubuntu2004 (virtualbox, 4.1.14)
  ```
  #### initialize & create a virtualbox VM from image file, start VM
  ```
  - vagrant.exe init generic/ubuntu2004
  - vagrant.exe up
  ```
  #### login into VM
  ```
  vagrant ssh
  ```
