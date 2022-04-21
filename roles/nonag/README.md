# nonag

Remove the "No valid subscription" windows that says "You do not have a valid subscription for this server. Please visit www.proxmox.com to get a list of available options." after logging into a Proxmox server WebUI.

Credit to John McLaren for originally posting this at https://johnscs.com/remove-proxmox51-subscription-notice/

## Requirements

None.

## Role Variables

None.

## Dependencies

None.

## Example Playbook

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
