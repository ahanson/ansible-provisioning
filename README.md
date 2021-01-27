# Ansible Desktop Provisioning:
* An Ansible Pull playbook for setting up Linux Mint Desktops.
* Based on [Jay LaCroix](https://jaylacroix.com/)' Ansible tutorials.
* Maybe it replaces the [FreeGeek Chicago](https://freegeekchicago.org/) [install script](https://github.com/freegeekchicago/fgc-installscript)? 
## Notes:
How to gather_facts on the target machine:

    ansible localhost -m setup

How to run the script on the target machine;

    sudo ansible-pull -U https://github.com/ahanson/ansible-provisioning.git
