yasarlaro.kvm
=========

Installs KVM hypervisor on supported operating systems.

Requirements
------------

Server has to support CPU virtualization and has be one of the below operating systems:
 - CentOS 7
 - CentOS 8
 - Ubuntu 18.x
 - Ubuntu 20.x

Role Variables
--------------

Role variables can be found under `vars` directory. Variable files are importanted based on the operationg system. If you would like to use a non-root user as the virtualization administrator, please take a look `vars/main.yaml` file and change it if needed.

Dependencies
------------

There is no dependency for this tole

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: yasarlaro.kvm }

License
-------

MIT License
