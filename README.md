Ansible Role: Etcd
=========

An Ansible role that installs clustered Etcd on your systemd enabled linux servers

Requirements
------------

- Ansible
- Docker
- Python
- Systemd

Role Variables
--------------

See `defaults/main.yml`

Dependencies
------------

None

Example Playbook
----------------

```yaml
- name: Import etcd role
  hosts: all
  become: true
  roles:
    - ansible-etcd
```

License
-------

BSD

Author Information
------------------
