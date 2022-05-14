# Proceso de instalación y ejecución de Docker Doom

El primer paso a realizar es el de buscar un link para el archivo que tenemos que usar dado que el link está actualmente caído o eliminado. He usado la página Wayback Machine para lograr obtener dicho comprimido.

## Descompresión del archivo

Usando el comando `tar -vzxf dockerdoomd.tar.gz` se descomprimirá el archivo, dado resultado a los archivos *dockerdoomd* y *dockerfile*

## Instalando el cliente VNC

Como nos dice en el repositorio original, necesitamos un cliente VNC para poder visualizar correctamente nuestro videojuego DOOM. 

Para este ejercicio, se hará uso de Vinagre, un cliente VNC completo y perfecto para nuestro objetivo. 
Se instala con el siguiente comando: `sudo apt install vinagre`

## Puesta en marcha de DOOM

Realizaremos el siguiente comando para iniciar los contenedores `for i in {1..4} ; do docker run -d -t ubuntu:14.04; done`. Posteriormente, haremos uso de `./dockerdoomd`

## Conexión

La conexión usa el puerto 5900, y como es en local, la composición será localhost:5900

![imagen](https://user-images.githubusercontent.com/95173613/168450124-f466a310-17b3-4d9f-9b1a-c2f29c784500.png)

Con la contraseña `1234`

![imagen](https://user-images.githubusercontent.com/95173613/168450180-aa02ee6e-928a-492a-8566-a294e93687fc.png)

Y tendremos el siguiente resultado

![imagen](https://user-images.githubusercontent.com/95173613/168450208-b95d283a-4cf6-4d21-a6f3-7f832ea616ae.png)
