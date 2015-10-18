Description
============

This repository contains the cookbook to build mongodb virtual machine on
virtual vox using ``vagrant`` and ``ansible``.

Usage
======

To run the virtual machine, execute :

    vagrant up

To connect on the virtual machine with ssh, execute :

    vagrant ssh

To reexecute installation scripts, execute :

    vagrant provision

To stop the virtual machine, execute :

    vagrant halt

To reload the virtual machine, execute :

    vagrant reload

To remove the virtual machine from your disk, execute :

    vagrant destroy

Check playbook
==============

    make tests

If it doesn't work due to missing ``ansible`` or ``ansible-galaxy roles``, use :

    bash scripts/bootstrap-tests.sh

Resources
=========

* [Mongodb](https://www.mongodb.org/)
* [Virtual box](https://www.virtualbox.org/)
* [Vagrant](https://www.vagrantup.com/)
* [Ansible](http://www.ansible.com/)
