Ansible Role: Disable Root
=========

The only purpose of this role is to lock out the root account on a system (if not already the case).
This enforces the user of the system to use *sudo* which offers logging for all commands.

Requirements
------------

No specific requirements for this role.

Role Variables
--------------

No variables for this role.

Dependencies
------------

No dependencies from other roles required.

Example Playbook
----------------

Here is a simple example playbook to use this role:

```
hosts: all
user: myuser
become: true
roles:
  - { role: disableroot, tags: [ 'disableroot' ] }
```

License
-------

MIT / BSD

Author Information
------------------

My name is Gaétan. You can follow me on [Twitter](https://twitter.com/gaetanict)

Website: [ICT Pour Tous](https://www.ictpourtous.com)
