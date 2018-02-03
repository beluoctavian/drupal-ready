Ansible Role: Drupal-ready
=========

An Ansible Role that installs all packages required to run efficiently a Drupal website.

How to run:
1. Create the inventory.ini file:
```
[webservers]
94.130.58.71
```

2. Run the playbook
`ansible-playbook tasks/main.yml -i inventory.ini --user=username --ask-sudo-pass`

Requirements
------------

Install galaxy requirements:
`ansible-galaxy install -r requirements.yml`

Role Variables
--------------

@todo: A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

* kyungw00k.python27
* geerlingguy.firewall
* geerlingguy.security
* geerlingguy.mysql
* geerlingguy.apache
* geerlingguy.php
* geerlingguy.php-mysql
* geerlingguy.php-memcached
* geerlingguy.apache-php-fpm
* geerlingguy.certbot
* geerlingguy.git
* geerlingguy.drush

Example Playbook
----------------

@todo: Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

This role was created in 2017 by [Octavian Belu](https://www.octavianbelu.ro/)
