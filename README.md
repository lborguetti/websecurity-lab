# websecurity-lab

This project is a simple lab with PHP/MySQL web application vulnerable.

Environment is builded with Vagrant, VirtualBox Machine or Docker Container,
and provisioned with Ansible.

Don't use it in production.

## First install Requirements

- Install [Virtual Box][1] or [Docker][4]
- Install [Vagrant][2]
- Install [Ansible][3]

## Running

        git clone https://github.com/lborguetti/websecurity-lab
        cd websecurity-lab

### Provider with Docker Container

        cd vagrant-docker
        vagrant up

### Provider with VirtualBox Machine

        cd vagrant-virtualbox
        vagrant up


Point your browser for http://127.0.0.1:8080/dvwa/setup.php

Click on the 'Create / Reset Database' button below to create your database.

Default username = **admin**

Default password = **password**

Security Level default = **high**

## Environment contains

- Ubuntu trusty64.
- apache2 compile for source with CFLAGS="-DBIG_SECURITY_HOLE" (for running apache with root).
- php5 compile for source.
- [Damn Vulnerable Web Application (DVWA)][5].

## TODO

- Enable role nowasp - [NOWASP (Mutillidae)][6].

[1]:https://www.virtualbox.org
[2]:http://www.vagrantup.com
[3]:http://www.ansible.com
[4]:http://www.docker.io
[5]:http://www.dvwa.co.uk/
[6]:http://sourceforge.net/projects/mutillidae/
