oracle_java
=========

Installs desired Oracle Java build to target RedHat-based host.

Requirements
------------

- Ansible 2.4+
- RHEL/CentOS 7+

Role Variables
--------------

Set the Oracle JDK version, update, and build number
```
jdk:
  version: 8
  update: 131
  build: 11
```

Example Playbook
----------------
``` yaml
  ---
  - hosts: localhost
    roles:
      - oracle_java
```

References
-------

- [get_url module](http://docs.ansible.com/ansible/latest/modules/get_url_module.html)
- [yum module](http://docs.ansible.com/ansible/latest/modules/yum_module.html)
- [alternatives module](http://docs.ansible.com/ansible/latest/modules/alternatives_module.html)

Author Information
------------------

- Name: Andrew Kuttor
- Email: andrew.kuttor@gmail.com
