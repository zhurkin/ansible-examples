Hosts Edit
=========

Managing the /etc/hosts file

Role Variables
--------------

hosts_edit_hostname: []

Entries to add to /etc/hosts. By default, nothing is added.

Example Variables hosts_edit_hostname
----------------

    hosts_edit_hostname:
       - 127.0.0.1: test1.local.loc
       - 127.0.0.2: test2.local.loc
       - 127.0.0.3: test3.local.loc test3

hosts_edit_backup: yes
Сreate a backup copy of the file.
If the variable is not defined, the backup file is not created by default.

Example Playbook
----------------

    - hosts: server
      roles:
         - { role: hosts_edit }

License
-------


Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
