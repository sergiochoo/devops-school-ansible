Apache
=========

This role deploys Apache web server and opens necessary firewall ports

Requirements
------------

Ansible 2.9 and higher

Role Variables
--------------
# default version of Apache
version: httpd

# default dir for www files
dest_dir: /var/www/html

Example Playbook
----------------

---
- hosts: node1.example.com
  become: true
  roles:
    - apache
  vars:
    version: httpd = 2.4.37

License
-------

BSD

Author Information
------------------

Sergei Afanasenko for EPAM devops&cloud training