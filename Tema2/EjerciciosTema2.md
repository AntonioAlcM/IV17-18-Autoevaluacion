## Ejercicio 1
**Descargar y ejecutar las pruebas de alguno de los proyectos anteriores, y si sale todo bien, hacer un pull request a este proyecto con tests adicionales, si es que faltan (en el momento que se lea este tema).**  
[Enlace al pull request](https://github.com/JJ/tests-python/pull/2)
## Ejercicio 2
**Para la aplicación que se está haciendo, escribir una serie de aserciones y probar que efectivamente no fallan. Añadir tests para una nueva funcionalidad, probar que falla y escribir el código para que no lo haga (vamos, lo que viene siendo TDD).**  
[Enlace al repositorio donde he añadido la función de test](https://github.com/AntonioAlcM/tests-python)
## Ejercicio 3
**Convertir los tests unitarios anteriores con assert a programas de test y ejecutarlos desde mocha, usando descripciones del test y del grupo de test de forma correcta. Si hasta ahora no has subido el código que has venido realizando a GitHub, es el momento de hacerlo, porque lo vas a necesitar un poco más adelante.**
En django esto ya es directo basta con ejecutar la orden python manage.py test Calificar
## Ejercicio 4
**Instalar alguno de los entornos virtuales de node.js (o de cualquier otro lenguaje con el que se esté familiarizado) y, con ellos, instalar la última versión existente, la versión minor más actual de la 4.x y lo mismo para la 0.11 o alguna impar (de desarrollo).**  
Como estoy utilizando python, he instalado su entorno virtual. Para ello he usado el comando pip install --upgrade virtualenv
## Ejercicio 5
**Como ejercicio, algo ligeramente diferente: una web para calificar las empresas en las que hacen prácticas los alumnos.   Las acciones serían:**  
**1. Crear empresa**

**2. Listar calificaciones para cada empresa**

**3. Crear calificación y añadirla (comprobando que la persona no la haya añadido ya)**

**4. Borrar calificación (si se arrepiente o te denuncia la empresa o algo)**

**5. Hacer un ránking de empresas por calificación, por ejemplo**

**6. Crear un repositorio en GitHub para la librería y crear un pequeño programa que use algunas de sus funcionalidades.**  

**Si se quiere hacer con cualquier otra aplicación, también es válido. Se trata de hacer una aplicación simple que se pueda hacer rápidamente con un generador de aplicaciones como los que incluyen diferentes marcos MVC. Si cuesta mucho trabajo, simplemente prepara una aplicación que puedas usar más adelante en el resto de los ejercicios. **  
[Enlace al proyecto](https://github.com/AntonioAlcM/IVCalificarEmpresas.git)
## Ejercicio 6
**Ejecutar el programa en diferentes versiones del lenguaje. ¿Funciona en todas ellas?**  
Yo he usado python con django en principio si esta preparado para funcionar con la version 3 y 2 de python, el problema es que a veces da error cuando quieres cargar el proyecto con python3
## Ejercicio 7
**Crear una descripción del módulo usando package.json. En caso de que se trate de otro lenguaje, usar el método correspondiente.**  
Voy a explicar como se hace en el caso de python:
  1. Para exportar las dependencias usas el comando pip freeze > requirement.txt
  2. Para instalar las dependencias usas el comando pip install -r requirement.txt

## Ejercicio 8
**Automatizar con grunt, gulp u otra herramienta de gestión de tareas en Node la generación de documentación de la librería que se cree usando docco u otro sistema similar de generación de documentación. Previamente, por supuesto, habrá que documentar tal librería.**
Para generar la documentación voy a usar Sphinx.
1. Instalar sphinx con pip install sphinx  
![imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema2/Imagenes/ejercicio8.1.png?raw=true)  
2. Generar la documentación con  sphinx-quickstart  
![imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema2/Imagenes/ejercicio8.2.png?raw=true)  

## Ejercicio 9
**Haced los dos primeros pasos antes de pasar al tercero.**
  ![imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema2/Imagenes/ejercicio9.0.png?raw=true)  
  ![imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema2/Imagenes/ejercicio9.2.png?raw=true)  
