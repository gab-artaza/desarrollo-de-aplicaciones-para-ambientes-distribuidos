Este programa se ejecuta primero y se queda "esperando" a que alguien se conecte a él.

    Abre un puerto: Crea un ServerSocket en el puerto 5000. Es como abrir una puerta en tu computadora para que otros puedan tocar.

    Espera (Bloqueo): Con serverSocket.accept(), el programa se pausa. Se queda esperando hasta que un cliente se conecte.

    Acepta conexión: Cuando el cliente se conecta, imprime la dirección IP de donde viene la conexión.

    Crea canales de comunicación: Abre un canal de entrada (BufferedReader entrada) para leer lo que el cliente le diga, y un canal de salida (PrintWriter salida) para poder responderle.

    Lee el mensaje: Se queda esperando a leer una línea de texto enviada por el cliente (entrada.readLine()).

    Procesa y responde: Convierte el mensaje recibido a mayúsculas (toUpperCase()) y se lo envía de vuelta al cliente añadiendo el texto "RESPUESTA SERVIDOR: ".

    Cierra la conexión: Termina la conexión con ese cliente y el programa finaliza.

2. ClienteEco.java (El Cliente)

Este programa se ejecuta después y es el que toma la iniciativa para hablar con el servidor.

    Se conecta: Crea un Socket intentando conectarse a la IP 127.0.0.1 (que es tu propia computadora, también llamada localhost) en el puerto 5000 (la misma puerta que abrió el servidor).

    Crea canales de comunicación: Al igual que el servidor, abre un canal de salida para escribirle al servidor, y un canal de entrada para leer su respuesta.

    Envía el mensaje: Escribe el texto "hola mundo desde el cliente distribuido" y lo envía a través del canal de salida.

    Espera la respuesta: Se queda esperando (entrada.readLine()) hasta que el servidor le devuelva la respuesta.

    Muestra la respuesta: Imprime en la consola lo que el servidor le contestó (que será el mensaje en mayúsculas).

    Cierra la conexión: El programa finaliza.
