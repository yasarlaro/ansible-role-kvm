yasarlaro.kvm
=========

Installs KVM hypervisor on supported operating systems.

Requirements
------------

Server has to support CPU virtualization and has be one of the below operating systems:
 - CentOS 7
 - CentOS 8

Role Variables
--------------

Role variables can be found under "vars" directory. Variable files are importanted based on the operationg system.

Dependencies
------------

The role expects [ipaddr](https://docs.ansible.com/ansible/latest/user_guide/playbooks_filters_ipaddr.html) filter is installed on the source host. Filter can be installed by:

```bash
pip install netaddr
```

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: yasarlaro.kvm }

License
-------

MIT License
