ansible-role-filebeat-postfix-bounce
=========

Install and configure filebeat for sending bounce logs to logstash

Requirements
------------

Debian Jessie

Role Variables
--------------

* logstash_host
* logstash_port


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
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
