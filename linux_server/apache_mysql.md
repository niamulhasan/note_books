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


