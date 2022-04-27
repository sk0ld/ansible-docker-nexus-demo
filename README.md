Ansible playbook to build war artifact inside docker, push to nexus and publish on tomcat inside docker
=========

Short info
------------

Tested on Ubuntu 20.04

dev host is for preparation of war file with maven inside docker container

prod host is for publishing war file by tomcat inside docker container


Example of /etc/ansible/hosts
-----------------------------

```
[dev]
devserver1 ansible_host=your_ip_or_fqdn_devserver1

[prod]
prodserver1 ansible_host=your_ip_or_fqdn_prodserver1

