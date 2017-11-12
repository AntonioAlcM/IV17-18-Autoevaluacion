## Ejercicio 1  
**Instala LXC en tu versión de Linux favorita. Normalmente la versión en desarrollo, disponible tanto en GitHub como en el sitio web está bastante más avanzada; para evitar problemas sobre todo con las herramientas que vamos a ver más adelante, conviene que te instales la última versión y si es posible una igual o mayor a la 1.0.**  
Para instalar lxc, lo que hemos hecho ha sido bajarnos el tar de la página [oficial](https://linuxcontainers.org/lxc/downloads/) de lxc. Una vez descomprimido hemos seguido las intrucciones del archivo INSTALL.  
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema4/Imagenes/ejercicio1.0.png?raw=true)
## Ejercicio 2  
**Comprobar qué interfaces puente se han creado y explicarlos.**  
Para comprobar que se han creado los interfaces puente, nos vamos a la consola he introducimos el comando ifconfig.    
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema4/Imagenes/ejercicio2.0.png?raw=true)
## Ejercicio 3  
**1. Crear y ejecutar un contenedor basado en Debian.**
En esta [página](https://wiki.debian.org/LXC) podemos encontrar un listado de las imágenes que podemos instalar en lxc.  
Según la versión de lxc deberemos usar:

    lxc-create -t debian -n so-debian o lxc launch images:debian/stretch/amd64 so-debian

  ![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema4/Imagenes/ejercicio3.1.png?raw=true)
**2. Crear y ejecutar un contenedor basado en otra distribución, tal como Fedora. Nota En general, crear un contenedor basado en tu distribución y otro basado en otra que no sea la tuya. Fedora, al parecer, tiene problemas si estás en Ubuntu 13.04 o superior, así que en tal caso usa cualquier otra distro. Por ejemplo, Óscar Zafra ha logrado instalar Gentoo usando un script descargado desde su sitio, como indica en este comentario en el issue.**  
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema4/Imagenes/ejercicio3.2.png?raw=true)

## Ejercicio 4
**1. Instalar lxc-webpanel y usarlo para arrancar, parar y visualizar las máquinas virtuales que se tengan instaladas.**  
Para poder instalar lxc-webpanel es necesario tener instalado Flask. Por otra parte, también necesitas ser el usuario root.  
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema4/Imagenes/ejercicio4.png?raw=true)

**2. Desde el panel restringir los recursos que pueden usar: CPU shares, CPUs que se pueden usar (en sistemas multinúcleo) o cantidad de memoria.**  
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema4/Imagenes/ejercicio4.1.png?raw=true)
## Ejercicio 5
**1. Comparar las prestaciones de un servidor web en una jaula y el mismo servidor en un contenedor. Usar nginx.**  

## Ejercicio 6  
**Instalar docker.**  
Para instalar docker he seguido el siguiente [manual](https://www.digitalocean.com/community/tutorials/como-instalar-y-usar-docker-en-ubuntu-16-04-es).
## Ejercicio 7  
**1. Instalar a partir de docker una imagen alternativa de Ubuntu y alguna adicional, por ejemplo de CentOS.**  
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema4/Imagenes/ejercicio7.0.png?raw=true)
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema4/Imagenes/ejercicio7.1.png?raw=true)
**2. Buscar e instalar una imagen que incluya MongoDB.**  
Para instalar una imagen con MongoDB, primero haríamos una búsqueda en docker del tipo: sudo docker search MongoDB, nos saldrá un listado como el de la primera imagen del apartado anterior. En mi caso yo he instalado mongo, para ello he hecho sudo docker pull mongo
## Ejercicio 8  
**Crear un usuario propio e instalar nginx en el contenedor creado de esta forma.**
Para crear un usuario en el contenedor, entraremos en el contenedor como vemos en la imagen, también podemos entrar usando el comando:

      sudo docker run -i -t ubuntu /bin/bash.

Una vez dentro del mismo, crearemos el usuario con el comando adduser de linux.
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema4/Imagenes/ejercicio8.0.png?raw=true)  
Para instalar nginx, primero actualizaremos los repositorio con apt-get update y luego simplemente instalar nginx con apt-get install nginx.    
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema4/Imagenes/ejercicio8.1.png?raw=true)  

## Ejercicio 9  
**Crear a partir del contenedor anterior una imagen persistente con commit.**  
Para obtener el id del container, debemos ejecutar sudo docker ps -a
Para obtener la id larga es necesario ejecutar el comando

         sudo docker inspect 1d4518300cfc

Una vez obtenido el id largo, ya podemos hacer el comit, el commit sería así:

    sudo docker commit 1d4518300cfcd914f73c1d3cbe48e524ba6a781df4f2d7537024f93456a7337a copia-ubuntu

![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema4/Imagenes/ejercicio9.0.png?raw=true)
## Ejercicio 10  
**Crear una imagen con las herramientas necesarias para el proyecto de la asignatura sobre un sistema operativo de tu elección.**  
La información de como hacerlo lo podre el el archivo [README.md](https://github.com/AntonioAlcM/tfg_ugr/blob/master/README.md)
