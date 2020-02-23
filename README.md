grav
=========

Little role to install grav-admin cms on apache webserver.

Requirements
------------

To execute:
* Ansible >= 2.7

To execute tests:
* Molecule == 2.22
* LXD

Role Variables
--------------

The grav_version variable can be used to install a special version of grav-admin.
The grav_document_root variable contains the path to your web document directory.

Dependencies
------------

No dependencies.

Example Playbook
----------------

```
    - hosts: servers
      roles:
         - { role: grav }
      vars:
        - grav_version: "1.6.21"
        - grav_document_root: "/var/www/html/grav"

```


License
-------

GPLv2

Etc
------------------

Feedback is appreciated. I like to improve my understanding in Ansible
related topics.

ToDo
----
- [ ] Add opertunity to choose between grav and grav-admin package
- [ ] Enhance role with compose, to use grav cli
- [ ] Enhance role for more webservers
