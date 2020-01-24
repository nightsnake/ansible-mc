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

All the settings of mc are standard apart from color scheme. You can change it via `mc_color_scheme` variable. If you want to use the default color scheme, please live this variable blank.
