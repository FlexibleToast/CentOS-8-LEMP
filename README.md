# CentOS LEMP

This Ansible playbook will install and configure all the necessary packages to create a LEMP (Linux Nginx MariaDB PHP) stack in CentOS 8. 

## Configuration

Nginx will serve from `/usr/share/nginx/html`. PHP will have a test page at `/usr/share/nginx/html/info.php` once you have confirmed it is working you should deletethe test page.

## Required steps

Set the root password for the MariaDB by changing `changeme` in the vars/main.yml at line:
         
`db_root_password: changeme #Change this password for your site`
