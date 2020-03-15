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

for root user please use `mc_root_color_scheme`. It setting up separately, and not depends about user you chose.

In the `mc.ext.j2` template you will find the settings file for managing mc extensions (which program will use for different type of files).

Also please be noticed, that standard `eog` package will be installed among with mc.
