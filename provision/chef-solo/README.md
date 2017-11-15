## HITO 2 

### Se procedera a crea un servidor de datos en la nube con OwnCloud

![owncloud_logo](https://user-images.githubusercontent.com/32844919/32866305-5af6f106-ca67-11e7-93e3-6b1e5e02fa0a.png)


Owncloud es una aplicación de software libre que te permitirá crear un servidor de archivos en la nube, en el cuál podrás tener un almacén de imágenes, documentos o incluso tu música, datos a los que tendrás acceso desde cualquier lugar con internet.También podemos encontrar herramientas como editor de texto, reproductor o calendario.
Cuenta con aplicación para Android, iOS y cliente de escritorio para Linux, Windows y Mac OS X.

Los requerimientos son los siguientes:

Sistema operativo / Distribución	
* Ubuntu 16.04, Debian 7 and 8, SUSE Linux Enterprise Server 12 and 12 SP1, Red Hat Enterprise Linux/Centos 6.5 and 7
Base de datos	
* MySQL or MariaDB 5.5+, Oracle 11g, PostgreSQL, & SQLite
Servidor web	
* Apache 2.4 with mod_php
Versión de PHP	
* PHP (5.6+ or 7.0+)


Se creará una receta para provisionar el servidor Owncloud 

Con ayuda de la receta, lo primero que haremos será actualizar el sistema y la lista de repositorios.

Se provisiona con los siguientes servicios:

* php 
* Apache2
* Sql-server


En la  Ruta /home/javer/chef/cookbooks

* 1.- Crear un directorio "owncloud" 

* 2.- Crear un directorio "recipes"

* 3.- Crear un archivo "default.rb"

![imagen 1](https://user-images.githubusercontent.com/32844919/32694355-eb5f805a-c73d-11e7-8eea-dac39e24a22c.JPG)

* 4.- En el archivo "default.rb" escribimos lo siguiente:

![imagen 2](https://user-images.githubusercontent.com/32844919/32694363-3389c0fc-c73e-11e7-8741-f676379b2897.JPG)

* 5.- Ejecutamos el comando 
```
sudo chef-solo -c ~/chef/solo.rb
```

![imagen 3](https://user-images.githubusercontent.com/32844919/32694373-762a0278-c73e-11e7-93ad-a2dfc3eb744a.JPG)

Podemos visualizar que se provisiono correctamente los servicios que necesitamos
