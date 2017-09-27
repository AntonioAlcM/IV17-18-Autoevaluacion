## Ejercicio 1

**Consultar en el catálogo de alguna tienda de informática el precio de un ordenador tipo servidor y calcular su coste de amortización a cuatro y siete años. Consultar este artículo en Infoautónomos sobre el tema.**
![Imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema1/Imagenes/servidor00.jpg?raw=true).  
 Los equipos informáticos se pueden amortizar como máximo un 25% del precio total. Se puede amortizar como mínimo en 4 años y como máximo en 8 años. Hay que tener en cuenta que las amortizaciones son por años naturales, si lo compras en el segundo semestre del año deducirás la parte proporcional a ese semestre.   
 [Tabla de amortizaciones](http://www.agenciatributaria.es/AEAT.internet/Inicio/_Segmentos_/Empresas_y_profesionales/Empresas/Impuesto_sobre_Sociedades/Periodos_impositivos_a_partir_de_1_1_2015/Base_imponible/Amortizacion/Tabla_de_coeficientes_de_amortizacion_lineal_.shtml).
1. **Amortización a cuatro años**.  
Teniendo en cuenta que el ordenador de tipo servidor ha costado 792.54, que podemos deducir el 25% de su precio y que lo hemos comprado el 1 de enero de 2017, las amortizaciones serían:
    * 2017: 198.135 euros.
    * 2018: 198.135 euros.
    * 2019: 198.135 euros.
    * 2020: 198.135 euros.
2. **Amortización a siete años**  
 Los dos primeros años amortizamos al 25% y el resto de años hasta llegar a los 7 años, se va reduciendo la amortización.  
    * 2017: 792.54 * 0,25 = 198.135 euros.
    * 2018: 792.54 * 0,25 = 198.135 euros.
    * 2019: 792.54 * 0,15 = 118.9 euros.
    * 2020: 792.54 * 0,15 = 118.9 euros.
    * 2021: 792.54 * 0,10 = 79.3 euros.
    * 2022: 792.54 * 0,05 = 39.6 euros.
    * 2023: 792.54 * 0,05 = 39.6 euros.

## Ejercicio 2  

**Usando las tablas de precios de servicios de alojamiento en Internet “clásicos”, es decir, que ofrezcan Virtual Private Servers o servidores físicos, y de proveedores de servicios en la nube, comparar el coste durante un año de un ordenador con un procesador estándar (escogerlo de forma que sea el mismo tipo de procesador en los dos vendedores) y con el resto de las características similares (tamaño de disco duro equivalente a transferencia de disco duro) en el caso de que la infraestructura comprada se usa sólo el 1% o el 10% del tiempo.**  
Para este ejercicio voy a comparar el costo de una máquina virtual en Azure y un servidor en Hostalia.
![imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema1/Imagenes/ejercicio2.0.jpg?raw=true).
![imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema1/Imagenes/ejercicio2.1.jpg?raw=true).  
El costo total en un año de un servidor de Hostalia es 99.9 * 3 meses + 299.9 * 9 meses = 2998.8 euros
1. Usando solo el 1% en un año.
  (0,688 * 24 horas * 30 días * 12 meses) * 0,01 = 59.44 euros
2. Usando solo el 10% en un año.
  (0,688 * 24 horas * 30 días * 12 meses) * 0,1 =  594.434 euros

## Ejercicio 3  
**En general, cualquier ordenador con menos de 5 o 6 años tendrá estos flags. ¿Qué modelo de procesador es?**   
Intel® Core™ i7-2670QM CPU @ 2.20GHz × 8    
**¿Qué aparece como salida de esa orden?**  
![imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema1/Imagenes/ejercicio3.0.png?raw=true)   
 **Si usas una máquina virtual, ¿qué resultado da?**  
No esta activa la virtualización.  
 **¿Y en una Raspberry Pi o, si tienes acceso, el procesador del móvil?**  
No esta activa la virtualización.  

## Ejercicio 4
**Comprobar si el núcleo instalado en tu ordenador contiene este módulo del kernel usando la orden kvm-ok.**  
![imagen](https://github.com/AntonioAlcM/IV17-18-Autoevaluacion/blob/master/Tema1/Imagenes/ejercicio4.0.png?raw=true)  
**Instalar un hipervisor para gestionar máquinas virtuales, que más adelante se podrá usar en pruebas y ejercicios.**  
sudo apt-get install virtualbox  

## Ejercicio 5  
**Darse de alta en servicios de nube usando ofertas gratuitas o cupones que pueda proporcionar el profesor.**  
Me he dado de alta en los servidores de Amazon con la cuenta de la ugr.  

## Ejercicio 6  
**Darse de alta en una web que permita hacer pruebas con alguno de los sistemas de gestión de nube anteriores.**    
En la página de la consola de amazon web service, podremos hacer distintas pruebas al servidor.
