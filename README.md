Ansible Role: Tower environement
=========

An Ansible Role that installs new virtual environments in Ansible Tower.

Requirements
------------

This should be compatible with both EL7 and EL8. 

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml` for all defaults):

```
venvs_parent_dir: /opt/custom_venv
venv_dir: "{{ venv_name }}"
venv_name: new_venv
venv_packages: 
  - ncclient
  - netadd
```

For the Ansible Tower username and password assign the variables below using a vault or credentials in tower:
```
toweruser: admin
towerpass: P@ssW0rd!
```

Dependencies
------------

None. 

Example Playbook
----------------
There is a playbook included with this role that does the required pre_task of pulling the current custom python environment paths, please refer to that as reference.

License
-------

BSD

Author Information
------------------

William Pat Martin