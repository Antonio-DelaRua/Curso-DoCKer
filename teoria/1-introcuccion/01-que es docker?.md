docker por definicion es una herramienta que permite desplegar aplicaciones en contenedores de forma rapida y portable, docker es capaz de generar aplicaciones de bolsillo debido a su estructura utiliza containers de imagenes, en una imagen defines toda la configuracion de todo el software, librerias y demas que necesita una aplicacion para funcionar y en un container lo vuelves realidad.


que significa esto? 

aplicaciones de bolsillo
desplegar y escalar aplicaciones
destruir y recrear

veamos un ejemplo : 

creando un server nuevo apache 

$ docker run -d -p 80 80 --name web httpd                 (docker run para crear un nuevo container, -d para ponerlo ultimo,p para el puerto,
                                                             nombre de la web y por ultimo la configuracion del container)


$ docker run -d -p 80:80 --name web httpd

para eliminarlo :

$ docker rm -fv web

//////////////////////////////////////////////////////////////

$ docker run -d -p 81:80 --name web2 nginx

para eliminarlo :

$ docker rm -fv web2
