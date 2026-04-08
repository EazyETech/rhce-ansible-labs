# Module 1 - Setting Up an Ansible Environment

## Overview
In this module, I set up an Ansible environment from scratch and used ad-hoc commands to manage and verify multiple Linux hosts.

## Skills Practiced
- Installing and configuring Ansible
- Creating a static inventory file
- Configuring ansible.cfg for project use
- Verifying connectivity using the ping module
- Running ad-hoc commands across host groups

## Key Tasks Completed
- Built a static inventory with host groups (webservers, balancers)
- Configured Ansible to use a local inventory file
- Disabled host key checking for lab environment
- Verified connectivity to all managed nodes
- Created users on target hosts using ad-hoc commands
- Created directories and files across host groups

## Example Commands Used
```bash
ansible all -m ping
ansible webservers -m user -a "name=testuser state=present"
