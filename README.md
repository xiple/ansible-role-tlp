Ansible role: TLP
=========

[![CI](https://github.com/xiple/ansible-role-tlp/actions/workflows/ci.yml/badge.svg)](https://github.com/xiple/ansible-role-tlp/actions/workflows/ci.yml)

An ansible role that installs TLP on Linux.

Requirements
----------------

None.

Role Variables
----------------

```yaml
tlp_custom_conf_manage: true
```

Installs xiple's custom configuration drop-in (see `files/01-mytlp.conf`).

Supported distributions
----------------

This role has been been developed and tested on the following distributions :

- Fedora : 43
- Debian : 13

Example Playbook
----------------

```yaml
- hosts: all
  vars:
    - tlp_custom_conf_manage: false
  roles:
    - xiple.tlp
```

License
-------

MIT
