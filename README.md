Satellite_Install
=========

Install all the required rpms and run the installation for satellite.

Requirements
------------

The host needs to be subscribed to the appropriate repositories.

Role Variables
--------------


Dependencies
------------
```
subscription-manager repos \
--enable=rhel-7-server-rpms \
--enable=rhel-server-rhscl-7-rpms \
--enable=rhel-7-server-satellite-6.3-rpms \
--enable=rhel-7-server-satellite-6.3-puppet4-rpms
```

Example Playbook
----------------


    - hosts: satellite
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

