# Ubuntu on NUC


## Install Ubuntu Server

### Boot USB in UEFI mode

English all (default settings, just hit enter)

* Hostname: ubuntu-nuc
* Username: nuc-user
* Password: root
* Use weak password - YES
* Encryption - No
* Force UEFI Install -YES


### If 64GB or more:
* use guided partition: use entire disk
* No proxy
* Install security updates automatically
* Install openSSH server and standard system utilities (use space to select)


### If 4GB model:
* Manual partition:
* Delete all partitions
* Create 150MB logical at beginning, use as EFI system partition area – bootable flag on
* Create 3.7GB primary at beginning, use as Ext4, mount point /, bootable flag off
* Create ~100 MB (rest of disk) logical at beginning, use as swap area – bootable flag off,
* Finish partition and write changes to disk


### Once booted:
* Connect your Arduino 101 with LCD to your Gateway device  
* After you log in with your credentials enter following commands to download and run the script:  
  `nuc-user@ubuntu-nuc:~# sudo apt-get install git curl npm`
  `nuc-user@ubuntu-nuc:~# git clone https://github.com/plangdon/iot-class.git`  
  `nuc-user@ubuntu-nuc:~# cd iot-class`   
  `nuc-user@ubuntu-nuc:~# cd installers/gateway-setup`  
  `nuc-user@ubuntu-nuc:~/gateway-setup# sudo ./ubuntu-gateway-setup.sh`  
* After script completes your system will reboot
