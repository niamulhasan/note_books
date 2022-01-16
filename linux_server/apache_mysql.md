# Installation with WSL2

## Install apache2

`sudo apt install apache2`

## Install mysql server

`sudo install mysql-server`

## Start apache2 and mysql server

`sudo service apache2 start`

`sudo service mysql start`

## Create an user for mysql with all privileges

Enter into the mysql command using
`sudo mysql`

then create an user using this command

`CREATE USER 'username'@'localhost' IDENTIFIED BY 'the_password';`

now give the full provilege to the user

`GRANT ALL PRIVILEGES ON *.* TO 'username'@'localhost' WITH GRANT OPTION;`



# Now for Laravel setup
I will install composer by running
`sudo apt install composer`



#(Optional Only for me)
I want to use vs code on my windows machine to edit server's files

Run this command to give premission to the vs code for editing file
`sudo chown -R user name /directory`








# Composer 2 for ububtu
sudo apt update
sudo apt install php-cli unzip
cd ~
curl -sS https://getcomposer.org/installer -o composer-setup.php

HASH=`curl -sS https://composer.github.io/installer.sig`
echo $HASH
php -r "if (hash_file('SHA384', 'composer-setup.php') === '$HASH') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
sudo php composer-setup.php --install-dir=/usr/local/bin --filename=composer
composer

apt search mbstring
sudo apt install php-mbstring


