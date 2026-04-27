# Module 4 - Handlers, Loops, Conditionals, and Jinja2 Templates

## Overview
This module focused on writing smarter and more efficient Ansible playbooks
using handlers, loops, conditionals, and Jinja2 templates.

## Skills Practiced
- Using handlers to trigger service actions only when changes occur
- Using loops with simple lists and dictionaries to manage multiple resources
- Using conditionals to control task execution based on host groups and facts
- Using Jinja2 templates to generate dynamic files

## Playbooks Included
- `httpd_setup.yml` - Installs httpd and starts it via handler when index.html changes
- `create_users_loop.yml` - Creates users using a simple loop list
- `create_advanced_users.yml` - Creates users using a loop with dictionaries
- `conditional_hostname.yml` - Creates a file only on hosts in the test group
- `check_memory.yml` - Displays memory info only if host has more than 1000MB RAM
- `set_motd.yml` - Deploys a dynamic MOTD using a Jinja2 template
- `generate_report.yml` - Generates a system report using a Jinja2 template
- `conditional_httpd_restart.yml` - Deploys Apache config conditionally and restarts httpd via handler

## Templates Included
- `motd.j2` - Jinja2 template with if/else for dev vs non-dev hosts
- `apache.conf.j2` - Apache config template using ansible_fqdn
- `system_report.j2` - System report template using Ansible facts

## Key Tasks Completed
- Installed and configured httpd with a handler-driven service start
- Created multiple users with both simple and dictionary-based loops
- Conditionally created files based on host group membership
- Used facts to conditionally display system memory
- Deployed dynamic MOTD with Jinja2 if/else logic
- Generated per-host system reports using Ansible facts
- Deployed Apache config only to webservers group with handler restart

## How to Run
```bash
ansible-playbook /home/automation/ansible1/httpd_setup.yml
ansible-playbook /home/automation/ansible1/create_users_loop.yml
ansible-playbook /home/automation/ansible1/create_advanced_users.yml
ansible-playbook /home/automation/ansible1/conditional_hostname.yml
ansible-playbook /home/automation/ansible1/check_memory.yml
ansible-playbook /home/automation/ansible1/set_motd.yml
ansible-playbook /home/automation/ansible1/generate_report.yml
ansible-playbook /home/automation/ansible1/conditional_httpd_restart.yml
```
