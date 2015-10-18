Description
============

This repository contains the cookbook to build mongodb virtual machine on
virtual vox using ``vagrant`` and ``ansible``.

Installation
=============

First clone this repository :

    git clone https://github.com/Esme-Sudria-Database/Vagrant-Mongodb.git

Then run the virtual machine, execute :

    cd Vagrant-Mongodb
    vagrant up

Using rockmongo
===============

Once the virtual machine provisioning done, use your browser to go on :

    http://192.168.33.10

The UserName:password to use is ``admin``:``admin``.

![Rockmongo login](https://cloud.githubusercontent.com/assets/159559/10564184/469ed9c6-75aa-11e5-998a-d9bbd6e20200.png)

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

Check playbook
==============

    make tests

If it doesn't work due to missing ``ansible`` or ``ansible-galaxy roles``, use :

    bash scripts/bootstrap-tests.sh

Resources
=========

* [Mongodb](https://www.mongodb.org/)
* [Rockmongo](http://rockmongo.com/)
* [Virtual box](https://www.virtualbox.org/)
* [Vagrant](https://www.vagrantup.com/)
* [Ansible](http://www.ansible.com/)
