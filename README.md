# Proyecto-TJBot_txt
manual del ejercicio TJBot en texto
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>PROYECTO TJ BOT</title>
<link rel="stylesheet" href="style_pagina_word_TJ.css">
</head>
<body>
<div id = "titulo1"> 2.	PROYECTO TJ BOT </div>
<div id="linea1"> ______________________________________________________</div>
<div id="texto1">En esta sección vamos a juntar todo lo aprendido anteriormente para construir un TJBot con el <br>
que poder mantener una conversación. [6] </div>
<br> 
<br>
<br>
<div id="texto2">Para ello vamos a utilizar una Raspberry Pi3, la cual conectaremos a los servicios de conversación <br>
de Watson y así poder hacer hablar a nuestro robot.</div>
<img id="img1" src="imagenes/Imagen1.png"> <br>
<p id="texto3"> El objetivo final será hacer que nuestro TJBot sea capaz de mantener una conversación con nosotros y obedezca algunas órdenes.</p>
<p id = "titulo2"> 1.1.	CÓMO CREAR A TJBOT </p>
<div id="linea2"> ______________________________________________________</div>
<p> 1.1.1.	RAPSBERRY PI3 </p>
<div> Raspberry Pi es un computador de placa única. <br> <br> <br>
Para trabajar con la Raspberry Pi3 vamos a necesitar un  <br>
monitor, un ratón, un teclado y una fuente de <br>
alimentación para trabajar con ella. También debemos <br>
tener una tarjeta micro SD con el sistema operativo <br>
instalado, en este caso trabajaremos con el sistema <br>
operativo Raspbian.
</div>
<div> <img src="imagenes/Imagen2.png"></div>
<div> Para crear nuestro TJBot hace falta conectar algunos componentes más a nuestra placa: </div>
<div> 
<li type="disc">Un micrófono</li>
<li type="disc">Un altavoz</li>
<li type="disc">Una cámara</li>
<li type="disc">Un servomotor</li>
<li type="disc">LED</li>
</div>
<div> 1.2.	MONTANDO A TJBOT </div>
<div> 
Para comenzar a trabajar con TJBot, lo primero que debemos hacer es obtener las piezas para poder montarlo.
<br> <br>
Este robot es DY (Do it yourself) y puede conseguirse imprimiendo las piezas en una impresora
3D. Las piezas que se deben imprimir pueden encontrarse en la siguiente web:
<br> <br> <br> 
<a href="https://ibmtjbot.github.io/#gettj"> https://ibmtjbot.github.io/#gettj</a> <br> <br> <br>
Las piezas que conseguiremos serán las siguientes: <br> <br>
<img src="imagenes/Imagen3.png"> <br>
¿Cómo lo montamos? <br> <br>
Primero, insertamos las piernas en la mandíbula. Las piernas entran en los agujeros en forma de <br>
L en la mandíbula. Inserta desde la parte superior de la mandíbula hacia abajo. <br> <br>
<img src="imagenes/Imagen4.png"> <br>
Después, cogemos la pieza "leg brace". Se encuentra en los dos orificios rectangulares en las <br>
patas debajo de la mandíbula. Mantiene las piernas rectas y soporta la mandíbula. Debemos <br>
asegurar que esté orientada de modo que haga contacto con la parte inferior de la mandíbula.<br>
<img src="imagenes/Imagen5.png"> <br>
Ahora, cogemos los pies y los insertamos en las muescas de la pierna como se muestra a <br>
continuación. Inserta los pies desde el exterior de cada pierna. <br>
<img src="imagenes/Imagen6.png"> <br>
Si tenemos un servo motor, es hora de insertarlo en el orificio del lado izquierdo en la mandíbula. <br>
Cogemos el retenedor inferior y lo deslizamos hacia abajo a través de los agujeros en forma de L en las patas. <br>
Los brazos de soporte en la parte inferior de este retenedor deben caber en las muescas de acoplamiento en la mandíbula. <br>
<img src="imagenes/Imagen7.png"> <br>
A continuación, insertaremos la Raspberry Pi. Se monta boca abajo, con sus puertos expuestos a través de los tres agujeros en la mandíbula.

Si tenemos una cámara: tomamos el soporte de montaje de la cámara. Deslizamos los dos montajes laterales de la 
cámara en las muescas en la parte delantera del retenedor. Deslizamos la cámara Pi en el soporte y luego agregue los 
reforzadores superior y frontal para mantener la cámara ajustada. <br>
<img src="imagenes/Imagen8.png"> <br>
El siguiente retenedor es el que tiene el pequeño círculo grabado en él. Lo añadimos a TJBot deslizándolo a través de 
los orificios en forma de L, con el círculo pequeño orientado hacia la derecha. Deslizamos el retenedor hacia abajo 
hasta que se encuentre con la parte superior de la Raspberry Pi.<br>
<img src="imagenes/Imagen9.png"> <br>
Insertamos el LED en el orificio central del retenedor pequeño. <br>
<img src="imagenes/Imagen10.png"> <br>
Por último, colocamos la cabeza. <br>
<img src="imagenes/Imagen11.png"> <br>
¡Ya está listo nuestro TJBot! <br>
</div>
<div> 1.2.1. CÓMO CONECTAR LOS COMPONENTES </div>
<div>A continuación, se muestra un esquema de la conexión de los diferentes componentes electrónicos que forman parte de nuestro TJBot. <br>
<img src="imagenes/Imagen12.png"> <br> <br>
</div>
<div> 1.3.	SERVICIOS DE WATSON</div>
<div> Para realizar el proyecto final del TJBot, vamos a utilizar tres servicios de Watson: Text to Speech,<br>
 Speech to Text y Watson Assistant.</div>
<div> 1.3.1.	TEXT TO SPEECH</div>
<div> El servicio Text to Speech proporciona una interfaz de programación de aplicaciones que utiliza  <br>
las capacidades de síntesis de voz de IBM para convertir texto escrito en voz de sonido natural. <br> <br> <br>
Para crear un servicio Text to Speech de Watson, debemos buscarlo en el catálogo de IBM Cloud. <br>
</div>
<img src="imagenes/Imagen13.png"> <br> <br>
<div> Una vez seleccionado el servicio deseado, le damos al botón de "Crear" para poder empezar a trabajar.</div>
<img src="imagenes/Imagen14.png"> <br> <br>
<div> Cuando ya tenemos nuestro servicio creado, podemos acceder a él desde nuestro Dashboard.</div>
<img src="imagenes/Imagen15.png"> <br> <br>
<div> En el apartado Service credentials (credenciales del servicio) podemos ver nuestro usuario y <br>
contraseña, que necesitaremos incluir más adelantes cuando configuremos el servicio Text to <br>
Speech en nuestra Raspberry Pi3.</div>
<div> ¡Hemos creado nuestro servicio Text to Speech! </div>
<div> 1.3.2.	SPEECH TO TEXT</div>
<div> Para crear un servicio Speech to Text de Watson, debemos buscarlo en el catálogo de IBM Cloud.</div>
<img src="imagenes/Imagen16.png"> <br> <br>
<div> Una vez seleccionado el servicio deseado, le damos al botón de "Crear" para poder empezar a trabajar.</div>
<img src="imagenes/Imagen17.png"> <br> <br>
<div> Cuando ya tenemos nuestro servicio creado, podemos acceder a él desde nuestro Dashboard.</div>
<img src="imagenes/Imagen18.png"> <br> <br>
<div> 
En el apartado Service credentials (credenciales del servicio) podemos ver nuestro usuario y <br>
contraseña, que necesitaremos incluir más adelantes cuando configuremos el servicio Speech to <br>
Text en nuestra Raspberry Pi3.
</div>
<div>¡Hemos creado nuestro servicio Speech to Text!</div>
<div> 1.3.3.	ASSISTANT</div>
<div> Para crear un servicio de Watson Assistant, debemos buscar el servicio deseado en el catálogo de IBM Cloud.</div>
<img src="imagenes/Imagen19.png"> <br> <br>
<div> Una vez seleccionado el servicio Assistant, le damos al botón de "Crear" para poder empezar a trabajar.</div>
<img src="imagenes/Imagen20.png"> <br> <br>
<div> Cuando ya tenemos nuestro servicio creado, podemos acceder a él desde nuestro Dashboard.
Una vez la página principal de nuestro servicio, debemos buscar el botón "Launch tool" que nos llevará a la herramienta en la que 
configuraremos y desarrollaremos nuestra conversación.
En el apartado Service credentials (credenciales del servicio) podemos ver nuestro usuario y contraseña, que necesitaremos incluir 
más adelantes cuando configuremos el servicio Assistant en nuestra Raspberry Pi3.
</div>
<div> 1.4.	CONFIGURAR A TJBOT</div>
<div> 1.4.1.	CONFIGURAR LA RASPBERRY PI 3</div>
<div> Como ya hemos mencionado, Raspberry Pi es similar a un computador completo, lo que significa que se necesita un monitor, 
ratón y teclado para utilizarla. [1]
Se puede conectar a un televisor a través de un cable HDMI.
También será necesario conectar la Raspberry a la Wifi.
En la mayoría de los kits Pi, la tarjeta SD ya está precargada con una imagen del sistema operativo Raspberry Pi. 
Se debe colocar la tarjeta SD en la Pi, encender la Pi y seguir las instrucciones en la pantalla para completar la instalación 
del sistema operativo.
Una vez tenemos todo preparado, hay que configurar los paquetes para empezar a trabajar.
Abrimos un terminal en el Pi y ejecutamos los siguientes comandos para instalar la última versión de Node.js y npm 
(Node Package Manager). Necesitará estos paquetes más tarde para ejecutar su código.
Para ello utilizamos el siguiente comando:
curl -sL http://ibm.biz/tjbot-bootstrap | sudo sh -
A continuación, será necesario configurar la salida de audio; el audio puede tener 2 opciones:
HDMI o Jack.
Abrimos un terminar, y escribimos el siguiente comando, para abrir la configuración de las Raspberry:
sudo raspi-config
</div>
<img src="imagenes/Imagen21.png"> <br> <br>
<div> Seleccionamos "Opciones avanzadas" y luego seleccionamos "Audio". Elegimos el canal correcto <br>
para el audio de salida. Si hemos conectado un altavoz externo a la toma de audio, debemos seleccionar la toma de 3,5 mm.
</div>
<img src="imagenes/Imagen22.png"> <br> <br>
<div> 1.4.2.	OBTENER EL CÓDIGO PARA TJBOT </div>
<div> Una vez tenemos todo configurado, necesitamos descargar el código base para el TJBot. <br>
Podemos hacerlo mediante los siguientes comandos:
git clone https://github.com/ibmtjbot/tjbot.git cd tjbot/recipes/conversation
npm install
Una vez tenemos el código instalado, tenemos que empezar a configurar los servicios de Watson. <br>
Como ya hemos dicho, los servicios que vamos a utilizar son 3: Text to Speech, Assistant y Speech to Text.
</div>
<img src="imagenes/Imagen23.png"> <br> <br>
<div> Recordemos que los tres servicios estaban ya creados; ahora lo único que necesitaremos serán <br>
las credenciales para poder añadirlas al código de configuración del TJBot.
Necesitamos abrir el archivo config.js para actualizar dicha información. Para ello, primero <br>
hacemos una copia del archivo original (config.default.js) mediante el siguiente comando:
cp config.default.js config.js
Una vez hecho, abrimos el archive config.js y actualizamos las credenciales de los servicios.
Será necesaria la password, el username y en el caso de Watson Assistant, el WorkspaceID.
</div>
<img src="imagenes/Imagen24.png"> <br> <br>
<div> 1.4.3.	PROBANDO A TJBOT</div>
<div> Una vez tenemos todo configurado y la conversación creada, podemos probar a TJBot.
Abrimos el terminal y ejecutamos el siguiente comando:
sudo node conversation.js
</div>
<div> ¡Ya puedes hablar con TJBot!</div>
</body>
</html>
