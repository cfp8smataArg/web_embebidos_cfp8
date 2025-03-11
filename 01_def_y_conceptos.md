---
layout: default
title: 01_def_y_conceptos
description: definiciones y conceptos relacionados con el curso
---

# Definiciones y conceptos generales

## ¿Qué es un sistema embebido?

![componentes](./assets/img/01_1raParte.jpg)

Un Sistema Embebido es un sistema electrónico diseñado para realizar pocas funciones en tiempo real, al contrario de lo que ocurre con las computadoras, las cuales tienen un propósito general, ya que están diseñadas para cubrir un amplio rango de necesidades, los Sistemas Embebidos se diseñan para cubrir necesidades específicas.

En un Sistema Embebido la mayoría de los componentes se encuentran incluidos en la placa base (la placa de video, audio, módem) y muchas veces los dispositivos resultantes no tienen el aspecto de lo que se suele asociar a una computadora. Algunos ejemplos de Sistemas Embebidos podrían ser dispositivos como un sistema de control de acceso, la electrónica que controla una máquina expendedora o el sistema de control de una fotocopiadora entre otras múltiples aplicaciones.

El Sistema Embebido suele tener en una de sus partes una computadora con características especiales conocida como microcontrolador que viene a ser el cerebro del sistema. Este no es más que un microprocesador que incluye interfaces de entrada/salida en el mismo chip. Normalmente estos sistemas poseen una interfaz externa para efectuar un monitoreo del estado y hacer un diagnóstico del sistema.

![componentes](./assets/img/02_1raParte.jpg)

## Qué es una placa Arduino? Qué es una placa ESP32?

![componentes](./assets/img/03_1raParte.png)

Este chip, en sus versiones dentro de placas de desarrollo, se ha popularizado muchisimo en toda la comunidad de electrónicos y desarrolladores. Se han desarrollado firmwares, documentación, herramientas y en la actualidad es fácil encontrar tutoriales sobre el mismo y continuamente se publican nuevos artículos.

Por supuesto, los fabricantes están atentos y han desarrollado numerosas placas de desarrollo que integran el ESP32. Cada vez aparecen nuevas opciones, algunas realmente interesantes.

También empiezan a verse artículos y productos comerciales que emplean el ESP32 como núcleo. 

En resumen, es un dispositivo muy interesante, con muchas aplicaciones y muy bajo costo. Tiene un potencial enorme para elaborar todo tipo de proyectos, sobre por su capacidad de comunicación, ocupando un lugar destacado en aplicaciones de IoT.

## Qué es un lenguaje de programación?

![componentes](./assets/img/04_1raParte.jpg)

Un lenguaje de programación es un conjunto de reglas y sintaxis que permite a los programadores dar instrucciones a una computadora para realizar tareas específicas.

Estos lenguajes actúan como un puente entre los humanos y las máquinas, facilitando la creación de software, aplicaciones y sistemas que ejecutan las instrucciones definidas en el código.

Los lenguajes de programación pueden dividirse en lenguajes de bajo nivel y lenguajes de alto nivel. Los lenguajes de bajo nivel, como el lenguaje de máquina, son directamente entendidos por la computadora, pero son difíciles de escribir y entender para los humanos, ya que se componen de largas cadenas de unos y ceros. Estos lenguajes permiten un control detallado del hardware, pero su complejidad los hace poco prácticos para el desarrollo cotidiano.

Por otro lado, los lenguajes de alto nivel como Python o Java son mucho más cercanos al lenguaje humano, lo que los hace más accesibles y fáciles de aprender. Estos lenguajes permiten escribir código que es traducido a lenguaje de máquina mediante compiladores o intérpretes, facilitando la creación de aplicaciones de manera más rápida y eficiente.

![componentes](./assets/img/05_1raParte.png)

Los lenguajes compilados e interpretados difieren en la forma en que se ejecuta el código. Un compilador toma el código fuente completo y lo convierte en código máquina antes de ejecutarlo, como sucede en lenguajes como _C_ o _C++_.

En cambio, un intérprete lee y ejecuta el código línea por línea, como ocurre en lenguajes como _Python_ o _JavaScript_.

En el caso de los sistemas embebidos, pueden ser programados directamente en el lenguaje ensamblador del microcontrolador o microprocesador o utilizando otros lenguajes como _C_ o _C++_ mediante compiladores específicos

![componentes](./assets/img/06_1raParte.jpg)

## Qué es un IDE?

Un entorno de desarrollo integrado (IDE) es una aplicación de software que ayuda a los programadores a desarrollar código de software de manera eficiente. Aumenta la productividad de los desarrolladores al combinar capacidades como editar, crear, probar y empaquetar software en una aplicación fácil de usar. Así como los escritores utilizan editores de texto y los contables, hojas de cálculo, los desarrolladores de software utilizan IDE para facilitar su trabajo. En el curso usaremos dos IDEs: **Arduino IDE** y **Visual Studio Code** con una extensión llamada **Platformio IDE**

## Programar con **Arduino IDE**

Ambas placas de desarrollo pueden programarse mediante el software __Arduino IDE__. En el caso de que no lo tengas instalado, visitá el anexo de este sitio web para ver el paso a paso.

### Si queremos programar una placa Arduino...

En la parte de menú tenemos una zona para acceder a funciones como carga de archivos, edición del texto del código, carga de librerías y ejemplos, configuración, herramientas, etc. En los botones de acceso rápido tenemos los siguientes iconos:

![componentes](./assets/img/07_1raParte.png)

![componentes](./assets/img/06a_1raParte.png) Verifica si tu programa está bien escrito y puede funcionar.

![componentes](./assets/img/06b_1raParte.png) Carga el programa a la placa de Arduino tras compilarlo.

![componentes](./assets/img/06c_1raParte.png) Crea un programa nuevo.

![componentes](./assets/img/06d_1raParte.png) Abre un programa.

![componentes](./assets/img/06e_1raParte.png) Guarda el programa en el disco duro de la computadora.

![componentes](./assets/img/06f_1raParte.png) (En la parte derecha de la barra de herramientas se encuentra el Monitor Serial) Abre una ventana de comunicación con la placa Arduino en la que podemos ver las respuestas que nuestro Arduino nos está dando, siempre que tengamos el USB conectado.

En el cuadro del editor de texto escribiremos el código del programa que queramos que Arduino ejecute.

Finalmente, en el área de mensajes y la consola Arduino nos irá dando información sobre si la consola está compilando, cargando y sobre los fallos o errores que se produzcan tanto en el código como en el propio IDE.

El siguiente paso que realizaremos será configurar nuestro IDE para que se comunique con nuestra placa Arduino. Para ello conectaremos nuestro Arduino mediante el cable USB a la PC y después de que el sistema operativo haya reconocido e instalado la tarjeta automáticamente, nos dirigimos a la zona de Menú, pulsamos en Herramientas y después en Tarjeta. Ahí seleccionamos el modelo de tarjeta Arduino que tengamos, en nuestro caso _Arduino UNO_.

![componentes](./assets/img/08_1raParte.png)

Después vamos a la opción Puerto Serial y elegimos el COM en el que tenemos conectado.

![componentes](./assets/img/09_1raParte.png)

Si nos aparecieran varios _COM_ activos, porque estamos usando otros dispositivos serial o por otro motivo, para saber cuál de ellos es el que se comunica con nuestra placa, solo tenemos que ir a Panel de control/Hardware/Administrador de dispositivos. Miramos la pestaña (Puertos _COM y _LPT_) y ahí nos aparecerá nuestro Arduino y el COM en el que está conectado. Con esto, ya podemos empezar a programar nuestro Arduino.

Para finalizar, probaremos que todo está correctamente instalado y configurado ejecutando nuestro primer programa, el más simple, el típico "HELLO WORLD" ("HOLA MUNDO"). Para ello solo tenés que copiar el siguiente código en la zona del editor de texto del _IDE Arduino_:

### Si queremos programar una placa ESP32...

El ESP32 no viene incluido en el IDE de Arduino por defecto, pero podemos agregarlo fácilmente utilizando el “Gestor de tarjetas”. Para esto, seguimos los siguientes pasos:

* Abrir el _Arduino IDE_ e ir a _Archivo > Preferencias_. En el campo _URLs adicionales de gestor de tarjetas_, añade la siguiente URL: __https://espressif.github.io/arduino-esp32/package_esp32_index.json__
* Luego, vamos a _Herramientas > Placa > Gestor de tarjetas_
* En el panel que aparece, buscamos _ESP32_ en la barra de búsqueda, y hacemos click en _Instalar_ en el paquete que aparece.
* Una vez completada la instalación, ya podés elegir los modelos de ESP32 en el desplegable, y estarás listo para programar el _ESP32_.

## Programar con **Visual Studio Code + Platformio IDE**

En un inicio, se utilizará el asistente (wizard) para crear un proyecto rápido y fácil.

* Para eso, ir a la pestaña de bienvenida de la extensión PlatformIO definida como: _PIO HOME_, luego hacer click en _crear proyecto_.
* Si no la encontrás, hacer click en el icono de la barra de tareas inferior con forma de _casa_.

![componentes](./assets/img/13_1raParte.png)

* Debes elegir un nombre para tu proyecto en PlatformIO.
* Luego, elegir la placa _Board_ (entre más de 1000 disponibles). Solo ingresa las primeras letras para que el listado se reduzca hasta encontrar la adecuada.
* En la última parte, la opción “framework” se indica automáticamente cuando eliges tu placa, aunque puedes elegir el que prefieras.

El Framework Arduino es un entorno de trabajo que representa el criterio, los conceptos, las buenas prácticas de programación, que se establecen como normas para que sea más fácil el desarrollo.

Un _SDK_ (kit de desarrollo de software) es similar a un framework, pero se orienta al desarrollo con un hardware exclusivo.

Para dar un ejemplo, el NODE MCU ESP8266 puede ser programado con el framework Arduino o con el SDK de Espressif.

Por otro lado, si se verifica la casilla “location”, entonces PlatformIO considera guardar el proyecto en una ubicación por defecto, aunque puedes elegir la que tu quieras.

![componentes](./assets/img/14_1raParte.png)

Una vez que presiones _finish_ el entorno comienza a buscar los archivos de soporte necesario, por ello tendrás que esperar un momento.

Una de las diferencias más grandes con el _IDE Arduino_ o el _IDE Arduino 2.0_ son los archivos que se crean con cada nuevo proyecto y la manera como se organizan. 

En el lateral izquierdo debes elegir el icono _Explorer_. En él, vas a encontrar el proyecto ordenado en carpetas desplegables que creó el asistente de _PlatformIO_. 

Cada carpeta y archivo, lógicamente cumple una tarea. Puede ser un tanto abrumador, aunque lo cierto, es que no es necesario entender cada uno al detalle, por ello, a continuación, verás los más importantes.

![componentes](./assets/img/15_1raParte.png)


1. _Espacio de trabajo_: en «Open Editors» vas a encontrar los archivos que están abiertos, mientras que «workspace» contiene el proyecto en el que estés trabajando actualmente, puedes agregar más de uno y eliminarlos sin problemas.
2. _Directorio del proyecto_: es la carpeta principal que contiene los archivos y subcarpetas que PlatformIO crea automáticamente. Puede haber más de uno según la cantidad de proyectos que se estén gestionando.
3. _Librerías_: en esta carpeta el gestor de librerías de PlatformIO incluye las librerías privadas de cada proyecto.
4. _Código principal_: la carpeta SCR (simboliza la abreviatura de “Source”, fuente en inglés) aquí se incluye el código principal o código fuente de nuestro proyecto.  Por otro lado, PlatformIO crea un fichero con el nombre “main.cpp”. Este es el equivalente al archivo compilado por el IDE Arduino llamado: “codigo.ino”.
5. _platformio.ini_: es un archivo de configuración que dota de funcionalidades extras al entorno. Es capaz de agilizar el trabajo cuando se trata de grandes proyectos.

### Si queremos programar una placa Arduino...

En primer lugar, recurre a la página de bienvenida, luego haz clic en crear proyecto. Debes dar un nombre al proyecto y elegir la placa. Por lo general, se usa el framework Arduino pero tu elige el que desees. 

Para programar un proyecto debes editar el código fuente “main.cpp”

![componentes](./assets/img/16_1raParte.png)














_yay_

[Ir al inicio](./index.html)
