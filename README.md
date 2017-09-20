JDK 8 Ansible Playbook
=========

This role downloads and installs JBoss 7.1.1

Requirements
------------

None

Role Variables
--------------

This role requires the following variables to be defined elsewhere in the playbook that uses it:
```yaml
  jboss_home:                 # JBoss install dir
  http_port:                  # JBoss port for http connections
  https_port:                 # JBoss port for https connections
```

Dependencies
------------

None

Example Playbook
----------------

Register the role in requirements.yml:
```yaml
- src: capitanh.jboss-ansible-role
  name: jboss
```
Include it in your playbooks:
```yaml
- hosts: servers
  roles:
    - jboss
```

License
-------

BSD

