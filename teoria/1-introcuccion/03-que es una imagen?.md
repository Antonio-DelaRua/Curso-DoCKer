___________________________________________________________________________________________________
|                                                                                                   |
|                                      IMAGENES                                                     | 
|                                                                                                   |
|                                                                                                   | 
|                                                                                                   |
|         ______________________________________________________________________________         _  |
|    ___  |                                                                             |         | | 
|   |     |                         Capa3-CMD                                           |         | |  
|   |  d  |                                                                             |         | |
|   |  o  |_____________________________________________________________________________|         | |
|   |  c  |                                                                             |         | |   
|  <   k  |                         Capa2-RUN                                           |   RO    > |
|   |  e  |                                                                             |         | |
|   |  r  |_____________________________________________________________________________|         | |
|   |  f  |                                                                             |         | |   
|   |  i  |                         Capa1-FROM                                          |         | | 
|   |  l  |                                                                             |        _| |
|   |  e  |_____________________________________________________________________________|           | 
|   |___                                                                                            |
|___________________________________________________________________________________________________|




¿que es una imagen de docker?

una imagen en docker es un paquete q contiene un rectangulo que embarca o que aborda, que contiene toda la configuracion necesaria para que funcione el servicio.

las imagenes se componen por capas la primera capa normalmente tienen un from signfica dentro de la imagen que sistema operativo voy a utilizar, aqui hemos hecho un ejemplo con 3 capas pero un container puede contener muchas mas capas, en la capa dos de esta imagen tenemos un run, la instruccion run significa que va a haber despues del sistema operativo como apache etc... y la 3 capa va a contener el cmd y esto es la linea que va a ejecutar el contenedor.

estas capas dentro de la imagen son de solo lectura es decir que yo no puedo modificar una capa, puedo seguir agregando capas encimas de las existentes.

estas capas se crean utilizando un archivo que se llama dockerfile dentro del dockerfile empezamos a definir las capas que queramos en este caso 3 capas.

el dockerfile es un archivo de texto plano que se llama dockerfile ( se puede llamar de otras maneras ) pero este es el archivo por default que va a buscar.


DOCKERFILE

FROM ubuntu:22         -------------------capa1

RUN yum -y install httod  ----------------capa2

CMD ["apachectl","-DFOREGROUND"]  --------capa3


es importante tener el cmd que se ejecute en primer plano .

