Duologic.carbon-relay-ng
========================

This role configures and installs carbon-relay-ng with the OS package manager. Tested CentOS 7.

Requirements
-----------

You probably need to add a repository that has the carbon-relay-ng package for your distribution. I've used raintaink's PackageCloud. See the example Playbook.

Role Variables
--------------

See [defaults/main.yml](defaults/main.yml)

Example Playbook
----------------

```
    - hosts: servers
      roles:
         - { role: packagecloud, repository: raintank/raintank, os: centos, version: 7 }
         - { role: Duologic.carbon-relay-ng }
```

License
-------

MIT

Author Information
------------------

Jeroen Op 't Eynde, jeroen@simplistic.be
