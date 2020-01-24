Midnight Commander ansible role
=========

Role for install mc with ansible

Typical playbook
```
- hosts: all
  become: yes
  gather_facts: yes
  roles:
    - mc
  tags: mc
```  
