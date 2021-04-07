# project-14
Dependences to be installed
* General
- yum install -y https://dl.fedoraproject.org/pub/epel/epel-release-latest-8.noarch.rpm
- yum install -y dnf-utils http://rpms.remirepo.net/enterprise/remi-release-8.rpm
- yum install python3 
- yum module reset php 
- yum module enable php:remi-7.4 
- yum install python3-pip
- python3 -m install --upgrade setuptools
- python3 -m install --upgrade pip


* For Mysql Database
- python3 -m pip install PyMySQL
- python3 -m pip install MySQLdb
- ansible-galaxy collection install community.mysql

* For Postgresql Database
- python3 -m pip install python-psycopg2

* For Posix Firewalld
- ansible-galaxy collection install ansible.posix

* For PHP related process
- yum --enablerepo=remi install php-phpunit-phploc
- yum  install php-xdebug
- yum -y install wget
- wget https://getcomposer.org/installer -O composer-installer.php
- php composer-installer.php --filename=composer --install-dir=/usr/local/bin 