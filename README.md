Description
============

This repository contains the cookbook to build mongodb virtual machine on
virtual vox using ``vagrant`` and ``ansible``.

Installation
=============

First clone this repository :

    git clone https://github.com/Esme-Sudria-Database/vagrant-mongodb.git

Then run the virtual machine, execute :

    cd vagrant-mongodb
    vagrant up

You can use [robomongo](https://robomongo.org/) to connect and use the database

Vagrant usage
==============

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

Resources
=========

* [Mongodb](https://www.mongodb.org/)
* [Robomongo](https://robomongo.org)
* [Rockmongo](http://rockmongo.com/)
* [Virtual box](https://www.virtualbox.org/)
* [Vagrant](https://www.vagrantup.com/)
* [Ansible](http://www.ansible.com/)
