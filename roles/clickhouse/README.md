ansible-clickhouse 
=========
![Build Status](https://github.com/alexeysetevoi/ansible-clickhouse/actions/workflows/ci.yml/badge.svg?branch=master)
[![Build Status](https://travis-ci.org/AlexeySetevoi/ansible-clickhouse.svg?branch=master)](https://travis-ci.org/github/AlexeySetevoi/ansible-clickhouse)
[![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/alexeysetevoi/ansible-clickhouse)](https://galaxy.ansible.com/alexeysetevoi/clickhouse)
[![Ansible Galaxy](https://img.shields.io/badge/role-alexeysetevoi.clickhouse-blue.svg)](https://galaxy.ansible.com/alexeysetevoi/clickhouse/)

Simple clickhouse-server deploy and management role.
Any issues and pr are welcome.

Role Variables
--------------
```yaml
clickhouse_version: "23.4.6.25"
```

F: You can manage listen ports
```yaml
clickhouse_http_port: 8123
clickhouse_tcp_port: 9000
clickhouse_interserver_http: 9009
```
F: You can add listen ips on top of defaults:
```yaml
clickhouse_listen_host_custom:
  - "192.168.0.1"
```

Example Playbook
- hosts: servers
  roles:
     - { role: clickhouse }
License
----
MIT

Author Information
------------------
Elena Volgina
[ClickHouse](https://clickhouse.com/docs/en/index.html) by [ClickHouse, Inc.](https://clickhouse.com/company/).

Role by [AlexeySetevoi](https://github.com/AlexeySetevoi).

Dear contributors, thank you.
