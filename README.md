Ansible Role: Etcd
=========

An Ansible role that installs clustered Etcd on your systemd enabled linux servers with automated certificate generation for mTLS.

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

Example Inventory
----------------

```ini
[etcd]
server1 ansible_host=192.168.88.223
server2 ansible_host=192.168.88.222
server3 ansible_host=192.168.88.224
```

License
-------

MIT

Author Information
------------------

Andrey Oschepkov