## Ejercicio 1    
**Instalar chef-solo en la máquina virtual que vayamos a usar**  
Para instalar chef usamos este comando:

      curl -L https://www.opscode.com/chef/install.sh | sudo bash
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema6/Imagenes/ejercicio1.0.png?raw=true)
## Ejercicio 2  
**Crear una receta para instalar la aplicación que se viene creando en la asignatura en alguna máquina virtual o servidor en la nube.**  


## Ejercicio 3  
**Desplegar la aplicación de DAI con todos los módulos necesarios usando un playbook de Ansible.**


## Ejercicio 4  
**Instalar una máquina virtual Debian usando Vagrant y conectar con ella.**
1. Instalamos la imagen de debian usando vagrant  
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema6/Imagenes/ejercicio4.0.png?raw=true)  
2. Creamos el vagrantfile de la imagen que acabamos de instalar  
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema6/Imagenes/ejercicio4.1.png?raw=true)
3. Levantamos la máquina  
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema6/Imagenes/ejercicio4.3.png?raw=true)
4. Nos conectamos la máquina por ssh para ello usamos el comando:
        vagrant ssh  
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema6/Imagenes/ejercicio4.4.png?raw=true)

## Ejercicio 5  
**Crear un script para provisionar nginx o cualquier otro servidor web que pueda ser útil para alguna otra práctica.**
1. Creamos el script     
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema6/Imagenes/ejercicio5.0.png?raw=true)
2. Aprovisionamos la máquina  
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema6/Imagenes/ejercicio5.1.png?raw=true)
3. Comprobamos que funciona
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema6/Imagenes/ejercicio5.3.png?raw=true)
## Ejercicio 6  
**Configurar tu máquina virtual usando vagrant con el provisionador chef.**  
