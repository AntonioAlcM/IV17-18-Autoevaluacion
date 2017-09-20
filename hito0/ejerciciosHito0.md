# Configurar acceso ssh en github

1. Creamos una clave ssh usando el algoritmo de encriptación rsa y como base usamos nuestro email de github.  
![img](IV17-18-Autoevaluacion/hito0/imagenes/CrearSSH00.jpg)
2. A continuación nos pedirá que le demos a intro si queremos guardar la clave en la carpeta por defecto, una vez dado a intro, nos solicitará introducir una contraseña para usar la clave ssh, si deseamos.  
En mi caso como ya la tenía creada, me ha pedido que si quería sobreescribirla.    ![img](IV17-18-Autoevaluacion/hito0/imagenes/CrearSSH01.jpg)
3. Lanzamos el ssh-agent en background.
4. Añadimos la clave privada ssh al ssh-agent.
5. Copiamos el contenido de la clave publica ssh en el portapapeles
6. Pinchamos en nuestro usuario y vamos al apartado setting.
![img](IV17-18-Autoevaluacion/hito0/imagenes/setting.png)
7. En el menú de la pagina settings  clickeamos en SSH and GPG keys.  ![img](IV17-18-Autoevaluacion/hito0/imagenes/menuSetting.jpg)
8. En la nueva ventana pinchamos en New SSH key or Add SSH key.  ![img](IV17-18-Autoevaluacion/hito0/imagenes/newssh.jpg)
9. En el formulario, rellenamos el campo title con una descripción de que dispositivo va a utilizar esa clave. En el campo de texto copiamos el contenido de la clave pública  ![img](IV17-18-Autoevaluacion/hito0/imagenes/ssh-key-paste.png)
11. Click Add SSH key.
12. Nos solicitará nuestra contraseña de Github para confirmar  
![img](IV17-18-Autoevaluacion/hito0/imagenes/sudo_mode_popup.png)

Ya esta configurado nuestro acceso ssh.
