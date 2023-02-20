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

This role is meant to be added as a dependency to other roles, that need to trigger a reboot and wait for the machine to be reachable again.

Add it to the other role's `meta/main.yml` file like so:

```yaml
[...]
dependencies:
  - role: 'johanneskastl.reboot'
```

Then you can notify this role's handlers from the other role's tasks:

```yaml
- name: Task that triggers a reboot
  [...]
  notify:
    - 'Reboot'
    - 'Wait for the machine(s) to be ready again'
```

License
-------

BSD-3-Clause

Author Information
------------------

I am Johannes Kastl, reachable via kastl@b1-systems.de.
