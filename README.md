# Ejercicio-de-Promocion-para-IP-2026
Es una "Juego" simple de consola desarrollada en Java como parte del desafío final de Introduccion a la Programación. El objetivo del juego es que el usuario logre adivinar un número aleatorio generado automáticamente por el sistema dentro de un rango de 1 a 50.


                         DETALLES DEL JUEGO


1. NOMBRE DEL JUEGO
¡Adivina el Número!


2. DESCRIPCION
Una aplicacion de consola desarrollada en Java donde el usuario debe 
adivinar un número aleatorio secreto generado por el sistema dentro de 
un rango y con un numero limitado de intentos.


3. FUNCIONALIDADES DEL PROYECTO + 1 FUNCION QUE NO SE PIDIO
* Generación de numeros aleatorios: El juego genera un número 
  aleatorio entre 1 y 50.

* Entrada de datos: Permite al usuario introducir su suposicion 
  usando la consola.

* Sugerencias: Informa al usuario si su numero introducido 
  es "demasiado alto" o "demasiado bajo".

* Control de intentos: El juego termina si el usuario agota sus 
  5 intentos permitidos.

* Revelaci0n del numero: Muestra el numero secreto si el usuario 
  no logra adivinarlo dentro de los límites del juego.


5. LIMITACIONES DEL PROYECTO
------------------------------------------------------------------------
* Modo de consola: Se juega a través de lineas de comandos; 
  no incluye interfaz gráfica.
* Validacion simple: El programa asume que el usuario introducirá 
  enteros validos. Por lo que si introduce letras
  el juego marcara un error y se cerrara.
* Sin persistencia: Los datos de la partida no se guardan al cerrar 
  el programa.


6. TRAMPA

                (aLGORITMO DE BuSQUEDA BINARIA)


Existe un método matemático para ganar siempre usando la menor cantidad 
de intentos posibles. Este método se llama Busqueda Binaria.

(Consiste en descartar la mitad de las opciones en cada intento.)


          EJEMPLO PRaCTICO DE JUEGO (buSQUEDA BINARIA)


Así se ve una partida real aplicando este método paso a paso:

¡Bienvenido al juego de Adivina el Número!
Estoy pensando en un número entre 1 y 50. Tienes 5 intentos.

* Intento 1:
  Introduce tu número: 25 (El centro exacto entre 1 y 50)
  El número es demasiado bajo. 
  -> [Lógica: Descartas del 1 al 25. Te quedan del 26 al 50]

* Intento 2:
  Introduce tu número: 37 (Sumas 12, que es la mitad de lo que queda)
  El número es demasiado bajo.
  -> [Lógica: Descartas del 26 al 37. Te quedan del 38 al 50]

* Intento 3:
  Introduce tu número: 44 (Sumas 6 o 7, el nuevo centro)
  El número es demasiado bajo.
  -> [Lógica: Descartas del 38 al 44. Te quedan del 45 al 50]

* Intento 4:
  Introduce tu número: 47 (Sumas 3, el nuevo centro)
  El número es demasiado bajo.
  -> [Lógica: Descartas del 45 al 47. Te quedan del 48 al 50]

* Intento 5:
  Introduce tu número: 49 (El centro entre 48 y 50)
  ¡Felicidades! ¡Adivinaste el número!

Al dividir el rango a la mitad de forma matemática en cada paso, 
llegamos al número exacto (49) justo en el último intento disponible.
