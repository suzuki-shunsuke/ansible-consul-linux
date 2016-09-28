consul-linux
==============

Install consul on Linux.

Requirements
------------

Nothing.

Role Variables
--------------

* consul_nonroot: Whether the remote_user is root or not. This variable is set automatically, and is used to execute tasks with the become option.

Dependencies
------------

Nothing.

Install
--------

Roles on Ansible Galaxy may be old,
so I recommend to install on GitHub([Advanced Downloading](https://galaxy.ansible.com/intro)).

```yaml
# roles.yml
- src: https://github.com/suzuki-shunsuke/ansible-consul-linux
  version: 1.0.0  # Please check the latest version
  name: suzuki-shunsuke.consul-linux
```

```
$ ansible-galaxy install -f -r roles.yml
```

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
