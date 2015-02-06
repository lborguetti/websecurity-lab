# websecurity.lab

This project is a simple lab with PHP/MySQL web application vulnerable.

Environment is builded with Vagrant, VirtualBox Machine and provisioned with Ansible.

Don't use it in production.

## First install Requirements

- Install [Virtual Box](https://www.virtualbox.org/)
- Install [Vagrant](http://www.vagrantup.com/)
- Install [Ansible](http://www.ansible.com/)

## Running

    git clone https://github.com/lborguetti/websecurity.lab
    cd websecurity.lab
    vagrant up

Point your browser for http://192.168.56.50/dvwa/setup.php or http://127.0.0.1:8080/dvwa/setup.php

Click on the 'Create / Reset Database' button below to create your database.

Default username = **admin**

Default password = **password**

Security Level default = **high**

## Environment contains

- Ubuntu trusty64.
- apache2 compile for source with CFLAGS="-DBIG_SECURITY_HOLE" (for running apache with root).
- php5 compile for source.
- [Damn Vulnerable Web Application (DVWA)](http://www.dvwa.co.uk/).

## TODO

- Add support for running in docker container.
- Enable role nowasp - [NOWASP (Mutillidae).](http://sourceforge.net/projects/mutillidae/)
