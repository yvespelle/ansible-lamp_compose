Role Name
=========

Ce playbook installe différents packages
- phpmyadmin
- mariadb-server
- apache2

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------
les variables database, user et password sont définies dans le fichier /etc/ansible/role/lamp_compose/default

le repertoire par défaut du projet (volume partagé): /opt
les ports et redirection des serices des containers: 
par défaut:
80 pour apache
8080 pour php my admin
3306 pour mariadb

Aedescriptiot of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Installation de Wordpress
-------------------------
l'hote de la base de donnée est :db

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
