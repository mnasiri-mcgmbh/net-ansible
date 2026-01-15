# net-ansible

Ansible project for configuring and updating network devices.

## Quick start
1. Install collections:
   ansible-galaxy collection install -r requirements.yml
2. Set vault secrets:
   ansible-vault edit inventories/lab/group_vars/vault.yml
3. Test:
   ansible-playbook playbooks/ping.yml --ask-vault-pass

## Structure
- inventories/ (lab, prod)
- playbooks/ (backup, deploy, upgrade)
- roles/ (vendor + common)
