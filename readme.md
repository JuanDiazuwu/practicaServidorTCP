# Práctica | Mi primer servidor TCP

Desarrollo Basado en Plataformas

## Unidad II

Conceptos Básicos de las Plataformas Web

## Lenguaje de Programación 

JavaScript (Node.js v18.13.0.)

## Autor

**Juan Antonio Díaz Fernández**

	Usuario: JuanDiazuwu

	Matricula: 348637

* Personal [Github](https://github.com/Fuan200/) 
* Escuela [Github](https://github.com/JuanDiazuwu)

## Funcionamiento

El archivo `client.js` se encarga de crear un cliente TCP.
El archivo `server.js` se encarga de crear un servidor TCP.

En `client.js` se importa la biblioteca `net`. Se establece una conexión con el servidor utilizando el método `connect` tomando como parámetros el puerto, la dirección ip, y una función flecha para saber si hay una conexión.
En el caso es el puerto `3000` y la dirección IP es `127.0.0.1`, lo que es conocido como localhost.
En caso de que la conexión se pierda es utlizado el evento `close`.
Además se registra un evento `data`, activado cuando se recibe datos del servidor.

En `client.js` se importa la biblioteca `net` utilizado para crear el servidor, el método llamado `createServer`. Se escucha en el puerto `3000` y la dirección IP es `127.0.0.1`  

## Instrucciones de uso

Para utilizar este script, sigue los siguiente pasos:

* 1 .- Clona el repositorio en tu maquina local.

* 2 .- Abre dos terminales en la raíz del repositorio clonado.

* 3 .- En la primera terminal, ejecuta el siguiente comando para iniciar el servidor TCP (se queda en modo de escucha):

```
node server.js
```

* 4 .- En la segunda terminal, ejecuta el siguiente terminal:

```
node client.js
```

* 5 .- Al ejecutar el punto 4 en la primera terminal aparecera un string con el siguiente contenido: `-------conexión-------`. 

* 6 .- En la segunda termianal se mostrara un mensaje: `....Conexión TCP Exitosa....`, lo que significa que el cliente se ha concetado correctamente al servidor.

* 7 .- Para terminar la conexión en cualquier treminal ejecute el comando `Ctrl + C`

Siéntete libre de clonar este repositorio y probar el funcionamiento del servidor. ¡Espero que te sea útil!