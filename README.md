Postgresql-Exporter
=========

This role installs binary postgres_exporter on Redhat-like system (any other OS with systemd should work too) from Github releases and allows access from prometheus servers

Requirements
------------

Server should have working PostgreSQL server with loaded `pg_stat_statements` shared library.

Example Playbook
----------------


```
- hosts: postgresql-exporter
  become: true
  roles:
    - role: postgresql-exporter
  tags:
    - postgresql-exporter
```

License
-------

MIT

Author Information
------------------

Anton Markelov