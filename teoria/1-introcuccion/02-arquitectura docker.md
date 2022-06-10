  
  
                                      ARQUITECTURA DE DOCKER
 ___________________________________________________________________________________________________
|                                                                                                   |
|                                           DOCKER HOST                                             | 
|                                                                                                   |
|                                                                                                   | 
|                                                                                                   |
|          Contenedor                 imagenes                volumenes               redes         |
|              |                          |                        |                     |          | 
|              |__________________________|________________________|_____________________|          |  
|              |_________________________________________________________________________|          |
|                                             |                                                     |
|                                             |                                                     | 
|                                             |                                                     |
|                                     DOCKER CLI- CLIENT                                            |
|                                                                                                   |
|                                         REST API                                                  |
|                                                                                                   | 
|                                    DOCKER DAEMON - SERVER                                         |
|___________________________________________________________________________________________________|



Toda la base se compone en el docker host, pero que es el docker host = si utilizamos una maquina de amazon e instalamos ese seria nuestro docker host, entonces digamos que el host hace referencia a la casa donde vive , o el servidor donde se aloja el servicio ese es el docker host. dentro de docker host vive el servicio mismo de docker que se llama docker daemon y es en realidad el que presta todos los servicios, es como un servicio mas del sistema.
Luego tenemos un api y tenemos un cliente. el cliente es la linea cuando vamos a ejecutar comandos donde quiera con la terminal nos conectamos donde quiera nos conectamos por medio de la api hacia el server y, por medio del server utiliza la api para contestarle al cliente. la api que se encuentra a la mitad no es mas que un canal de comunicacion entre dockers cliente y server. con el docker cli podemos manejar contenedores podemos manejar imagenes, volumenes y redes. en el fondo lo que va a hacer el cli es utilizar la api y se va a conectar al docker daemon que es quien presta el servicio de docker.




                                    \                                                                            /
