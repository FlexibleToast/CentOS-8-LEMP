# CentOS LEMP

This Ansible playbook will install and configure all the necessary packages to create a LEMP (Linux Nginx MariaDB PHP) stack in CentOS 8. 

## Configuration

Nginx will server from `/usr/share/nginx/html`. PHP will have a test page that you should delete at `/usr/share/nginx/html/info.php` once you have confirmed it is working.

## Required steps

Two changes are required to be made to the main playbook `main.yml`

1. Set the hostname of your server by changing `hostname` at the line:
   
      - `hosts: hostname #Change this to the host you require`

2. Set the root password for the MariaDB by changing `changeme` at the line:
         
      - `db_root_password: changeme #Change this password for your site`

## How to run

`ansible-playbook main.yml --ask-become-pass`
