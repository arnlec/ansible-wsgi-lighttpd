ansible-wsgi-lighttpd
=========

Use lighttpd as WSGI for a python application

Requirements
------------

None

Role Variables
--------------

- app_name: python package name
- module_name: module name to import in fcgi script 
- server_name: variable name to import in fcgi script
- python_version: default python version (default: 3)

Dependencies
------------

None

Example Playbook
----------------


    - hosts: servers
      roles:
         - { role: ansible-wsgi-lighttpd, app_name: my-python-package, module_name: my_python_module, server_name: my_variable_name }

License
-------

BSD

Author Information
------------------

arnaud@lecann.com
