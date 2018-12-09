Playbook install auto LEMP + Wordpress
- CentOS 7
- Nginx
- Mariadb
- PHP-FPM

sequence create roles in this playbook
- update and install epel-release

- install nginx and create vhost
- create user, group owner
- create fodler contains source and change owner
- start nginx

- install mariadb
- create user and database
- start mariadb

- install php-fpm
- copy config php-fpm.conf
- start php-fpm

- install wordpress (wget, unzip...)
- config connection string database
- chown user
