# Ansible Install Java
Script for installing java with gradle in Ansible

## Example

```yaml
- hosts: all
  become: true
  vars:
    java_version: "21"
    gradle_version: "8.10.2"

  tasks:
    - name: Install Java
      include_tasks: ./task/ansible_install_java/playbook.yml 
```