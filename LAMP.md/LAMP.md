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
NOTE: The step above will allow firewall for apache once it is enabled, it is important we allow firewall for ssh. ssh runs on port 22, if firewall is not allowed for ssh running on port 22, connection to the ubuntu instance via ssh will be permanently

    sudo ufw allow 22
    
To check if ubuntu instance has been installed successfully

    sudo systemctl status apache2

To access your web server on your browser

    http://ubuntu_instance_public_ip_address
An Apache default page will displayed. 
You can check your ubuntu instance ip address from your aws console from the EC2 instance service management or input the command below

    curl http://icanhazip.com

##                                        Installation of Mysql
