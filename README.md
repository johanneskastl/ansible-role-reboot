![Ansible Lint](https://github.com/johanneskastl/ansible-role-reboot/workflows/Ansible%20Lint/badge.svg)

reboot
=========

Reboot a node and wait until it comes up again.

Requirements
------------

None.

Role Variables
--------------

None.

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: 'johanneskastl.reboot' }

License
-------

BSD-3-Clause

Author Information
------------------

I am Johannes Kastl, reachable via kastl@b1-systems.de.
