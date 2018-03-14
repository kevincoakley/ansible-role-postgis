ansible-role-postgis
====================

[![Build Status](https://travis-ci.org/kevincoakley/ansible-role-postgis.svg?branch=master)](https://travis-ci.org/kevincoakley/ansible-role-postgis)

Install the PostGIS extension for Postgresql - https://postgis.net/ . Tested with Postgresql 10 on CentOS 7.

Requirements
------------

Postgresql 10

Role Variables
--------------

See defaults/main.yml and the example inventory below

Dependencies
------------

None

Example Playbook
----------------

    - name: Install PostGIS extension for Postgresql for CentOS
      hosts: postgis
      become: yes
      become_method: sudo
       
      roles:
        - ansible-role-postgis
    
      tags:
        - postgis

Example Inventory
-----------------
   
    [postgis]
    centos-system

License
-------

BSD

Author Information
------------------

Kevin Coakley (https://github.com/kevincoakley)