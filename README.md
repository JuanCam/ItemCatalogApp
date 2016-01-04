# ItemCatalogApp
Describes how to use the Catalog Application
<h4> Accesesing the server</h4><br>
The IP adress for the linux server is this one 52.35.52.60, the ssh port is 2200 and the key for authentication is udacity key.rsa.<br>
<h4> Url site </h4><br>
The Url for the website is 52.35.52.60-<br>
<h5> Setting up the server</h5>
First of all the <b>grader</b> user was created.<br>
The permission to sudo was given to the grader user, by creating a file inside the sudoers.d folder and adding grader ALL=(ALL:ALL) NOPASSWD:ALL, (NOPASSWD is for removing all password authentication whan a sudo oparation is performed). <br>
The default ssh port was changed in the sshd_config configuration file replacing the line 'Port 22' by 'Port 2200'.<br>
The firewall was set-up, first, by denying all incoming ports and then allowing only the 80 port for http (www), the 22 tcp port and the 123 port.<br>
Root login was disabled in the same sshd_config file, in the authentication line this content 'PermitRootLogin yes' was changed by this one 'PermitRootLogin no'<br>

<h4> General Usage Notes</h4><br>
The software consists of this web page - https://github.com/JuanCam/Item-Catalog. Is built up in Python-Flask and its Database system was changed from SQLite to PostgreSQL, the way of conecting to the postgres database in the app is this one postgresql://catalog:123@localhost:5432/catalog where catalog is the user and the database name and 123 is the password.<br>

<h4>Third party resources</h4><br>
- Setting up firewall on Ubuntu: https://www.digitalocean.com/community/tutorials/how-to-setup-a-firewall-with-ufw-on-an-ubuntu-and-debian-cloud-server<br>
- Install PostgreSQL on Ubuntu: https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-ubuntu-14-04
- Install Apache on Ubuntu: https://www.digitalocean.com/community/tutorials/how-to-configure-the-apache-web-server-on-an-ubuntu-or-debian-vps
- Setting up a flask application using Apache mod_wsgi: http://swaroopsm.github.io/12-02-2012-Deploying-Python-Flask-on-Apache-using-mod_wsgi.html
- The SqlAlchemy documentation for using PostgreSQL: http://www.sqlalchemy.org/
