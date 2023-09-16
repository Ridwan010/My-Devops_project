# LAMP STACK IMPLEMENTATION
The word LAMP refers to a group of open source software installed together which can be used to host web applications.
***LAMP*** meaning Linux; a unix operating system, Apache; a web server, Mysql; a database and PHP; an Hypertext preprocessor.

### Tools Used For Completion of the project
- An AWS account with an ubuntu EC2 instance
- Virtual machine using linux
- [SSH](https://www.digitalocean.com/community/tutorials/how-to-set-up-ssh-keys-on-ubuntu-20-04)

##                             Installation of Apache
update apt repositories

    sudo apt update
Install apache web server

    sudo apt install apache2
Allow firewall for apache

    sudo ufw allow in "Apache"
