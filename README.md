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

`keystone_hostname`:  Hostname/IP address of the controller node.
                      Defaults to "localhost".

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: horizon, keystone_hostname: localhost }

License
-------

Apache

Author Information
------------------

Davide Guerri - davide.guerri@gmail.com
