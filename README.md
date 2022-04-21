# Ansible Collection - engonzal.proxmox

This collection contains Proxmox roles used to manage proxmox servers.

It contains:
- nonag: role to remove the subscription prompt displayed after logging into the Proxmox WebUI

## Usage

Install the collection:

```bash
ansible-galaxy collection install engonzal.proxmox
```

Then you can use the roles in your playbook:

```yaml
- name: Proxmox
  hosts: lab
  remote_user: root
  collections:
    - engonzal.proxmox
  tasks:
    - import_role:
        name: nonag
```

## Author

This collection was create by Noe Gonzalez.