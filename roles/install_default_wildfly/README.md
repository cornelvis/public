Role Name
=========

install_default_wildfly

Role to install default wildfly on one or more hosts

Requirements
------------

Open connection to internet to download the instal file

Role Variables
--------------

var_wildfly_download_url
var_wildfly_dest_folder
var_wildfly_archive_dest
var_tmp_wildfly_dest_folder
var_group
var_user
var_wildfly_service_dest

Dependencies
------------

Written for Ubuntu (Debian)
works on ansible 2.10.8

Example Playbook
----------------

---
- name: install wildfly server
  gather_facts: false
  become: True
  become_user: root
  hosts: all

  roles:
    - install_default_wildfly

License
-------

GNU General Public License v3.0

Steps based on https://medium.com/@hasnat.saeed/install-jboss-wildfly-on-ubuntu-18-04-ac00719a2f02

Author Information
------------------

Cornelis van Ginkel
cornelvis[AT]gmail.com
