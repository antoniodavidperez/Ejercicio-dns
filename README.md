# Ejercicio-dns
## Creación de las máquinas
Creamos el raid 0 para el servidor dns.
![raid0_servidordns.PNG](./raid0_servidordns.PNG)

Creamos el raid 5 para el servidor web y ftp.
![raid5_servidorwebyftp.PNG](./raid5_servidorwebyftp.PNG)

## Creación del servidor DNS
Declarar las zonas de los sitios.
![named.conf.local.PNG](./named.conf.local.PNG)

Configurar los servidores DNS a los que va a acudir nuestro servidor en el caso de que nos conozca la IP del nombre por el que le están preguntando.
![named.conf.options.PNG](./named.conf.options.PNG)

Crear las zonas directas de cada sitio donde se relacionan las IP con los nombres.
![rd.sitioa.com.PNG](./rd.sitioa.com.PNG)
![rd.sitiob.net.PNG](./rd.sitiob.net.PNG)
![rd.sitioc.net.PNG](./rd.sitioc.net.PNG)

## Creación del servidor Apache
Crear los host virtuales, para ello hay que crear primero la estructura de carpetas y luego configurar los archivos.
![sitioa.com.conf.PNG](./sitioa.com.conf.PNG)
![sitiob.net.conf.PNG](./sitiob.net.conf.PNG)
![sitioc.net.conf.PNG](./sitioc.net.conf.PNG)

## Comprobación desde el lado del cliente
Comprobación de los host por el terminar de un cliente.
![comprobacionHost.PNG](./comprobacionHost.PNG)

Comprobación de los host en el navegador del cliente.
![navegadorSitioa.PNG](./navegadoraSitioa.PNG)
![navegadorSitiob.PNG](./navegadoraSitiob.PNG)
![navegadorSitioc.PNG](./navegadoraSitioc.PNG)
