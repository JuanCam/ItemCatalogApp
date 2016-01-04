# ItemCatalogApp
Describes how to use the Catalog Application
<h5> Accesesing the server</h5><br>
The IP adress for the linux server is this one 52.35.52.60, the ssh port is 2200 and the key for authentication is udacity key.rsa.<br>
<h5> Url site </h5><br>
The Url for the website is 52.35.52.60-<br>
<h5> General Usage Notes</h5><br>
The software consists of this web page - https://github.com/JuanCam/Item-Catalog. Is built up in Python-Flask and its Database system was changed from SQLite to PostgreSQL, the way of conecting to the postgres database in the app is this one postgresql://catalog:123@localhost:5432/catalog where catalog is the user and the database name and 123 is the password.<br>
<h5>Third party resources</h5><br>
- Setting up firewall on Ubuntu: https://www.digitalocean.com/community/tutorials/how-to-setup-a-firewall-with-ufw-on-an-ubuntu-and-debian-cloud-server<br>
- Install PostgreSQL on Ubuntu: https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-ubuntu-14-04
- Install Apache on Ubuntu: https://www.digitalocean.com/community/tutorials/how-to-configure-the-apache-web-server-on-an-ubuntu-or-debian-vps
- Setting up a flask application using Apache mod_wsgi: http://swaroopsm.github.io/12-02-2012-Deploying-Python-Flask-on-Apache-using-mod_wsgi.html
