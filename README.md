Ansible Role: Vagrant
=========

[![Build Status](https://travis-ci.org/patrick-hill/ansible-role-vagrant.svg?branch=master)](https://travis-ci.org/patrick-hill/ansible-role-vagrant)
[![Ansible Galaxy](https://img.shields.io/badge/ansible--galaxy-patrick--hill.vagrant-blue.svg)](https://galaxy.ansible.com/patrick-hill/vagrant)


Installs [Vagrant](https://www.vagrantup.com/) on Debian based OS and plugins


Requirements
------------

Ansible 2.0+

Role Variables
--------------

    vagrant_version
"vagrant_version" defines the version to install

    vagrant_plugins
"vagrant_plugins" list of vagrant plugins to install


Dependencies
------------

None.

Example Playbook
----------------

    - hosts: development-machines
      roles:
        - { role: patrick-hill.vagrant}

*Inside `defaults/main.yml`*:

    version: "1.9.1"
    plugins:
      - vagrant-hostmanager
      - vagrant-reload

License
-------

BSD

Author Information
------------------

Role written in 2016 by [Patrick Hill](http://www.HillsPCWorld.com) 
