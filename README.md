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

Dataset 
=======
The Data Sources used to build the dataset "cities15000.json" comes from http://www.geonames.org/data-sources.html. This work is licensed under a Creative Commons Attribution 3.0 License, see http://creativecommons.org/licenses/by/3.0/

To comply with the license terms, the dataset "cities15000.json" is also under a Creative Commons Attribution 3.0 License. 

The main 'cities' collection has the following keys:

Key | description
------------------|------------------
geonameid         | number, id of record in geonames database
name              | string, name of geographical point  
asciiname         | string, name of geographical point 
alternatenames    | array, alternate names of the city
coordinates       | array, longitude in decimal degrees (wgs84), latitude in decimal degrees (wgs84), elevation in meters (integer, optionnal) 
feature class     | string, see http://www.geonames.org/export/codes.html
feature code      | string, see http://www.geonames.org/export/codes.html 
country code      | string, ISO-3166 2-letter country code, 2 characters
cc2               | string, alternate country codes ISO-3166 2-letter country code
admin1 code       | string, fipscode (subject to change to iso code), see exceptions below
admin2 code       | string, code for the second administrative division, a county in the US
admin3 code       | string, code for third level administrative division
admin4 code       | string, code for fourth level administrative division
population        | number
dem               | string, digital elevation model, srtm3 or gtopo30, average elevation of 3''x3'' (ca 90mx90m) or 30''x30'' (ca 900mx900m) area in meters, integer. srtm processed by cgiar/ciat.
timezone          | string, the iana timezone id
modification date | date, date of last modification in yyyy-MM-dd format


AdminCodes:
Most adm1 are FIPS codes. ISO codes are used for US, CH, BE and ME. UK and Greece are using an additional level between country and fips code. The code '00' stands for general features where no specific adm1    code is defined.
The corresponding admin feature is found with the same countrycode and adminX codes and the respective feature code ADMx.




Resources
=========

* [Mongodb](https://www.mongodb.org/)
* [Robomongo](https://robomongo.org)
* [Rockmongo](http://rockmongo.com/)
* [Virtual box](https://www.virtualbox.org/)
* [Vagrant](https://www.vagrantup.com/)
* [Ansible](http://www.ansible.com/)
* [geoname](http://www.geonames.org/)
* [dataset meteo](https://www.ncei.noaa.gov/data/global-hourly/access/)
