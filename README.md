# Ansible Desktop Provisioning:
* An Ansible Pull playbook for setting up Linux Mint Desktops.
* Based on [Jay LaCroix](https://jaylacroix.com/)' series of [Ansible tutorials](https://www.youtube.com/playlist?list=PLT98CRl2KxKEUHie1m24-wkyHpEsa4Y70).
* Maybe it replaces the [FreeGeek Chicago](https://freegeekchicago.org/) [install script](https://github.com/freegeekchicago/fgc-installscript)? 

## Questions:
* How many different versions of Linux Mint should I test this on? 
    * Linux Mint 19.3 XFCE.
    * Linux Mint 20.01 XFCE.
* Should I test it on older versions of (x/k)Ubuntu? Older stuff sometimes comes in the door at Freegeek for support.
* Do we need the pepperflash player anymore, now that Flash has been retired?

## Done:
* Updating, upgrading, removing useless packages, emptying the package cache.
* Installing a short list of basic packages. 
* check if there's a webcam and install cheese.
* Make a initial Timeshift snapshot. Don't make another snapshot if there is already one snapshot.

## To Do:
* If it's Xubuntu, install xubuntu-restricted-extras, remove abiword and gnumeric.
* check if it's an Apple machine and act accordingly.
* Show the old-school steam locomotive ascii animation after everything is done.


## Notes:
You will need [Git](https://git-scm.com/) and [Ansible](https://www.ansible.com/) to run this script. Here's how to get them:

    sudo apt-get install git ansible

How to gather_facts on the target machine:

    ansible localhost -m setup

How to run the script on the target machine;

    sudo ansible-pull -U https://github.com/ahanson/ansible-provisioning.git
