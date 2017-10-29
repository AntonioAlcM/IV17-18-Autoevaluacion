## Ejercicio 1
**Darse de alta en algún servicio PaaS tal como Heroku, Nodejitsu, BlueMix u OpenShift.**
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema3/Imagenes/ejercicio1.png?raw=true)
## Ejercicio 2  
**Crear una aplicación en OpenShift o en algún otro PaaS en el que se haya dado uno de alta. Realizar un despliegue de prueba usando alguno de los ejemplos.**  
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema3/Imagenes/ejercicio2.0.png?raw=true)  
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema3/Imagenes/ejercicio2.1.png?raw=true)  
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema3/Imagenes/ejercicio2.2.png?raw=true)  
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema3/Imagenes/ejercicio2.3.png?raw=true)  
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema3/Imagenes/ejercicio2.4.png?raw=true)
## Ejercicio 3
**Realizar una app en express (o el lenguaje y marco elegido) que incluya variables como en el caso anterior.**  
Para este ejercicio voy a aprovechar una aplicación que hice en DAI. Es una aplicación creada en Flask. Esta aplicación consiste en introducir en la url un usuario y que salga un mensaje de hola, en caso de introducir una url no válida que te de un error 404

import sys  
reload(sys)  
sys.setdefaultencoding('utf8') #Sin esto da error de ascii

from flask import Flask, flash, request
app = Flask(__name__)
@app.route('/user/<username>')
def mostrarPerfilUsuario(username):
    return 'Hola %s' % username



@app.errorhandler(404)
def page_not_found(error):
    return "Página no encontrada", 404

if __name__ == '__main__':
    app.run(host='0.0.0.0', debug=True)

## Ejercicio 4
**Crear pruebas para las diferentes rutas de la aplicación.**  

import os
import ejercicio3
import unittest
import tempfile

class ejercicio3TestCase(unittest.TestCase):

    def setUp(self):
        self.db_fd, ejercicio3.app.config['DATABASE'] = tempfile.mkstemp()
        ejercicio3.app.config['TESTING'] = True
        self.app = ejercicio3.app.test_client()


    def tearDown(self):
        os.close(self.db_fd)
        os.unlink(ejercicio3.app.config['DATABASE'])

    def test_funciona(self):
        resultado = self.app.get('/user/juan')
        self.assertEqual(resultado.status_code, 200)

    def test_otro_enlace(self):
        resultado = self.app.get('/antonio')
        self.assertEqual(resultado.status_code, 404)

if __name__ == '__main__':
    unittest.main()

## Ejercicio 5
**Instalar y echar a andar tu primera aplicación en Heroku.**  
Las imagenes estan puestas en el ejercicio 2
## Ejercicio 6
**Usar como base la aplicación de ejemplo de heroku y combinarla con la aplicación en node que se ha creado anteriormente. Probarla de forma local con foreman. Al final de cada modificación, los tests tendrán que funcionar correctamente; cuando se pasen los tests, se puede volver a desplegar en heroku.**
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema3/Imagenes/ejercicio6.0.png?raw=true)
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema3/Imagenes/ejercicio6.1.png?raw=true)
## Ejercicio 7
**Haz alguna modificación a tu aplicación en node.js para Heroku, sin olvidar añadir los tests para la nueva funcionalidad, y configura el despliegue automático a Heroku usando Snap CI o alguno de los otros servicios, como Codeship, mencionados en StackOverflow**  
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema3/Imagenes/ejercicio7.0.png?raw=true)
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema3/Imagenes/ejercicio8.0.png?raw=true)
## Ejercicio 8  
**Preparar la aplicación con la que se ha venido trabajando hasta este momento para ejecutarse en un PaaS, el que se haya elegido.**  
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema3/Imagenes/ejercicio7.0.png?raw=true)
