## Ejercicio 1    
**Instalar los paquetes necesarios para usar KVM. Se pueden seguir estas instrucciones. Ya lo hicimos en el primer tema, pero volver a comprobar si nuestro sistema está preparado para ejecutarlo o hay que conformarse con la para virtualización.**  
1. Instalamos kvm con el siguiente comando  

        sudo apt install -y qemu-kvm libvirt-bin

2. Añadimos un usuario a kvm  

        sudo adduser antonio KVM

    ![imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema5/Imagenes/ejercicio1.png?raw=true)  

3. Comprobamos que nuestro sistema esta preparado para ejecutarlo  
![imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema5/Imagenes/ejercicio1.1.png?raw=true)

## Ejercicio 2    
**1. Crear varias máquinas virtuales con algún sistema operativo libre tal como Linux o BSD. Si se quieren distribuciones que ocupen poco espacio con el objetivo principalmente de hacer pruebas se puede usar CoreOS (que sirve como soporte para Docker) GALPon Minino, hecha en Galicia para el mundo, Damn Small Linux, SliTaz (que cabe en 35 megas) y ttylinux (basado en línea de órdenes solo).**
1. Creamos el hd
![imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema5/Imagenes/ejercicio2.1.png?raw=true)
2. Iniciamos la máquina virtual en el hd recien creado y cargando la imagen del sistema operativo
![imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema5/Imagenes/ejercicio2.1.1.png?raw=true)
3. Instalamos
![imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema5/Imagenes/ejercicio2.1.1.1.png?raw=true)
**2. Hacer un ejercicio equivalente usando otro hipervisor como Xen, VirtualBox o Parallels.**  
![imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema5/Imagenes/ejercicio2.2.png?raw=true)  

## Ejercicio 3  
**Crear un benchmark de velocidad de entrada salida y comprobar la diferencia entre usar paravirtualización y arrancar la máquina virtual simplemente con**
**qemu-system-x86_64 -hda /media/Backup/Isos/discovirtual.img**

## Ejercicio 4
**Crear una máquina virtual Linux con 512 megas de RAM y entorno gráfico LXDE a la que se pueda acceder mediante VNC y ssh.**  
1. Instalamos vnc con:

        sudo apt install -y vinagre

2. Para pode conectarnos a la máquina virtual con vnc ejecutaremos el siguiente comando, dicho comando activará vnc en la máquina virtual:

        qemu-system-x86_64 -vnc 0.0.0.0:1 -hda lubuntu.img
3. Ahora conectaremos con vnc utilizando:

        vinagre 0.0.0.1
4. Activaremos la opción para ssh

        qemu-system-x86_64 -hda lubuntu.img -m 512M -name antonio -redir tcp:22022::22

5. Accederemos por ssh

        ssh -p 22022 localhost
## Ejercicio 5     
**Crear una máquina virtual ubuntu e instalar en ella alguno de los servicios que estamos usando en el proyecto de la asignatura.**    
El proyecto usa como servicios redis y rabbitmq-server. Dichos servicios los instalaremos en un linux mint
![imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema5/Imagenes/ejercicio5.png?raw=true)  
## Ejercicio 6  
**Instalar una máquina virtual con Linux Mint para el hipervisor que tengas instalado.**  
Voy a instalar en virtualbox un linux Mint
![imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema5/Imagenes/ejercicio6.0.png?raw=true)  
![imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema5/Imagenes/ejercicio6.1.png?raw=true)  
