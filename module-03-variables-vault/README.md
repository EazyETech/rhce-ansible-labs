# Module 3 - Variables, Vault, and Ansible Facts

## Overview
This module focused on working with variables, securing sensitive data using Ansible Vault, and gathering system information using Ansible facts.

## Skills Practiced
- Defining variables in playbooks
- Using the debug module to display values
- Creating and using Ansible Vault files
- Securing user passwords
- Accessing and using Ansible facts
- Writing system information to files

## Playbooks Included
- variables.yml - Demonstrates variable usage
- secret_user.yml - Creates a secure user using Vault
- host_info.yml - Extracts system facts and writes them to a file

## Key Tasks Completed
- Defined variables within playbooks
- Used debug to print variable values
- Created encrypted Vault files
- Used hashed passwords for secure user creation
- Extracted hostname, FQDN, OS distribution, IP address, and BIOS version
- Stored system facts in a file

## How to Run
```bash
ansible-playbook variables.yml
ansible-playbook --ask-vault-pass secret_user.yml
ansible-playbook host_info.yml
