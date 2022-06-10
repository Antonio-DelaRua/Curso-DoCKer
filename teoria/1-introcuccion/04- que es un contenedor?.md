



____________________________________________________________________________________________________
|                                                                                                   | 
|                                                                                                   |
|                                   CONTENEDOR                                                      |
|                                                                                                   |
|                                                                                                   |
|                                 capa-4-EJECUCION                                                  |
|                                                                                                   |
|                                                                                                   |
|                                                                                                   |
|___________________________________________________________________________________________________|
|                                                                                                   |
|                                      IMAGENES                                                     | 
|                                                                                                   |
|                                                                                                   | 
|                                                                                                   |
|         ______________________________________________________________________________         _  |
|    ___  |                                                                             |         | | 
|   |     |                         Capa-3-CMD                                          |         | |  
|   |  d  |                                                                             |         | |
|   |  o  |_____________________________________________________________________________|         | |
|   |  c  |                                                                             |         | |   
|  <   k  |                         Capa-2-RUN                                          |   RO    > |
|   |  e  |                                                                             |         | |
|   |  r  |_____________________________________________________________________________|         | |
|   |  f  |                                                                             |         | |   
|   |  i  |                         Capa-1-FROM                                         |         | | 
|   |  l  |                                                                             |        _| |
|   |  e  |_____________________________________________________________________________|           | 
|   |___                                                                                            |
|___________________________________________________________________________________________________|




un contenedor es una capa adicional que lo que va a hacer es traer una ejecucion en tiempo real de las 3 capas. nuestro contenedor va a tener el sistema operativo de la capa 1 el from  la capa 2 dice que instalamos apache asi que el contenedor va a tener apache y el cmd es lo que va a necesitar el contendor para estar vivo .  la capa 4 si es de escritura , si estamos en la capa 4 podemos acceder a la capa 1-2-3 q no tienen escritura , pero todos los cambios que hagamos van a ser temporales , porque lo que modifiquemos no lo estamos modificando en la imagen sino solo en la capa4.

el contenedor tiene las capas de las imagenes (capa1-2-3) contiene  tambien volumenes , y por ultimo redes para lograr comunicar contenedores entre si etc..

