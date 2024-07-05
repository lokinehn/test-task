# Test task playbook


## Requirements
Require roles:
- disk-encryption
- cpu
- network

All required roles should store at roles_path = ./roles (or another path defined in ansible.cfg)

## Run playbook

To run playbook use command:
ansible-playbook -i inventories/test/inventory.yml main.yml (--tags={specified_tag}) (--user={user_name}) (--check --diff *to run in dry-run mode)
