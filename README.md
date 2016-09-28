consul-linux
==============

[![Build Status](https://travis-ci.org/suzuki-shunsuke/ansible-consul-linux.svg?branch=master)](https://travis-ci.org/suzuki-shunsuke/ansible-consul-linux)

Install consul on Linux.

https://galaxy.ansible.com/suzuki-shunsuke/consul-linux/

Requirements
------------

* unzip

Role Variables
--------------

* consul_nonroot: Whether the remote_user is root or not. This variable is set automatically, and is used to execute tasks with the become option.
* consul_version: The Consul version. The default value is 0.7.0.

Dependencies
------------

Nothing.

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
  - role: suzuki-shunsuke.consul-linux
```

License
-------

MIT
