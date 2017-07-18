ansible-role-filebeat-postfix-bounce
=========

Install and configure filebeat for sending bounce logs to a logstash (configured with this [role](https://github.com/web-education/ansible-role-logstash-postfix-bounce))

Requirements
------------

Debian Jessie

Role Variables
--------------

* logstash_host
* logstash_port


Example Playbook
----------------

```yaml
---
- name: 'install filebeat'
  hosts: mail-relays
  remote_user: root
  roles:
    - role: ansible-role-filebeat-postfix-bounce
      logstash_host: 'logstash.localdomain'
      logstash_port: 5044

```
License
-------

MIT
