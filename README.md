Horizon
=========

OpenStack Horizon dashboard installation

_Tested on Ubuntu Precise (12.04) and Trusty (14.04)_

Requirements
------------

apache2 and libapache2-mod-wsgi are needed.
They are installed by this role, if not found.

Role Variables
--------------

### Keystone (must exist)

| Name | Default value | Description | Note |
|---  |---  |---  |--- |
| `keystone_hostname` | `localhost` | Hostname/IP address of the controller node ||


Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: openstack-horizon, keystone_hostname: localhost }

---

A complete Ansible playbook demo, which uses this role, is available on Github (dguerri/vagrant-ansible-openstack) <https://github.com/dguerri/vagrant-ansible-openstack>

---


License
-------

Apache

Author Information
------------------

Davide Guerri - davide.guerri@gmail.com
