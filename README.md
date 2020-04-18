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
- init_function: init function 
- python_version: default python version (default: 3)

Dependencies
------------

None

Example Playbook
----------------


    - hosts: servers
      roles:
         - { role: ansible-wsgi-lighttpd, app_name: my-python-package, module_name: my_python_module, init_function: my_init_func }

License
-------

BSD

Author Information
------------------

arnaud@lecann.com
