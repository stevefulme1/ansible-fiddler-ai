# Getting Started with stevefulme1.fiddler_ai

>-

## Installation

```bash
ansible-galaxy collection install stevefulme1.fiddler_ai
```

## Requirements

- Ansible >= 2.16
- Python >= 3.12

## Authentication

Most modules require authentication credentials. Set these as variables
in your playbook, inventory, or Ansible Vault:

```yaml
vars:
  api_url: "https://your-service.example.com"
  api_token: "{{ vault_api_token }}"
  validate_certs: true
```

Store sensitive credentials in Ansible Vault:

```bash
ansible-vault encrypt_string 'your-token-here' --name 'vault_api_token'
```

## Quick Example

```yaml
---
- name: Example playbook
  hosts: localhost
  connection: local
  gather_facts: false
  collections:
    - stevefulme1.fiddler_ai
  tasks:
    - name: Get info
      stevefulme1.fiddler_ai.alert:
        api_url: "{{ api_url }}"
        api_token: "{{ api_token }}"
      register: result

    - name: Show result
      ansible.builtin.debug:
        var: result
```

## Collection Contents

- **Modules**: 12
- **Roles**: 2
- **EDA plugins**: 1

## Next Steps

- Browse the module documentation: `ansible-doc stevefulme1.fiddler_ai.<module_name>`
- Check the [README](../README.md) for the full module and role list
- Review [CONTRIBUTING.md](../CONTRIBUTING.md) to contribute
