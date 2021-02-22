# Ansible Desktop Provisioning:
* An Ansible Pull playbook for setting up Linux Mint Desktops.
* Based on [Jay LaCroix](https://jaylacroix.com/)' series of [Ansible tutorials](https://www.youtube.com/playlist?list=PLT98CRl2KxKEUHie1m24-wkyHpEsa4Y70).
* Maybe it replaces the [FreeGeek Chicago](https://freegeekchicago.org/) [install script](https://github.com/freegeekchicago/fgc-installscript)? 
## Notes:
You will need [Git](https://git-scm.com/) and [Ansible](https://www.ansible.com/) to run this script. Here's how to get them:

    sudo apt-get install git ansible

How to gather_facts on the target machine:

    ansible localhost -m setup

How to run the script on the target machine;

    sudo ansible-pull -U https://github.com/ahanson/ansible-provisioning.git
