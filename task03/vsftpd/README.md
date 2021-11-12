VSFTPD
=========

This role deploys VSFTPD ftp server and opens necessary firewall ports

- anonymous access is allowed to the /var/ftp/pub folder;
- allowed anonymous upload to the /var/ftp/pub/upload folder;
- the necessary permissions and the corresponding SELinux context are configured:
  "ftpd_anon_write" boolean - value "on".

Requirements
------------

Ansible 2.9 and higher

Role Variables
--------------
# default version of Apache
version: VSFTPD

Example Playbook
----------------

---
- hosts: node1.example.com
  become: true
  roles:
    - vsftpd
  vars:
    version: vsftpd = 3.0.3

License
-------

BSD

Author Information
------------------

Sergei Afanasenko for EPAM devops&cloud training