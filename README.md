Ansible Docker Role
=========
This role installs the current Edge build Docker CE using the offical repo, for more information on Docker CE see the offical site at [https://www.docker.com/community-edition](https://www.docker.com/community-edition).

Requirements
------------
Apart from requiring root access via `become: yes` this role has no special requirements.

Role Variables
--------------
All of the variables can be found in the `vars` folder.


Dependencies
------------
None.

Example Playbook
----------------
An example playbook can be found below;

```
- hosts: docker
  gather_facts: true
  become: yes
  become_method: sudo

  roles:
    - russmckendrick.docker
```

License
-------
BSD

Author Information
------------------
This role is published by [Russ McKendrick](http://russ.mckendrick.io/).