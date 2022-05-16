# Agregar un HTML personalizado a en servidor web dockerizado Nginx

## Instalación

En docker hub, buscaremos la imagen Nginx.

![imagen](https://user-images.githubusercontent.com/95173613/168653868-0c96fd61-5b62-4616-8204-236dab35ab21.png)

Nos dará el comando `docker pull nginx` para descargar la imagen de Nginx. En la terminal, de este caso Ubuntu, realizaremos dicho comando.

![imagen](https://user-images.githubusercontent.com/95173613/168654345-907bee8d-5b39-4e35-b718-ab55531f6229.png)

Y posteriormente el comando `docker run --rm -d -p 8080:80 --name web nginx` que será para iniciar nuestra imagen.
La ejecución del contenedor como demonio (-d), puerto 8080 en la red local y de nombre --name.

![imagen](https://user-images.githubusercontent.com/95173613/168654463-e9b8690f-fe0f-4866-84cd-f7489f5d215d.png)

Y el resultado final de la instalación sería este:

![imagen](https://user-images.githubusercontent.com/95173613/168654605-60188257-34fb-43ed-8f7d-1fec510c2741.png)

## Configuración

Ahora que ya tenemos Nginx puesto a punto y sabemos como funciona, vamos a configurarlo. De base, la ruta dónde buscará los html Nginx será en `/usr/share/nginx/html`, pero para comodiddad y no tener problemas, como nos recomienda el del repositorio origial, vamos a crear una carpeta llamada *Nginx* en documentos y dentro de esta crear una carpeta *site-content* para alojar nuestro html. El directorio final será `/home/jordiop/Documents/nginx/site-content`

Para el html, se nos solicita que aparezca nuestro nombre:

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Actividad Sistemas</title>
</head>
<body>
    <h1>Jordi Osarenkhoe Petro</h1>
</body>
</html>
```
Y guardarlo como index.html

Y realizaremos el siguiente comando:

`docker run --rm -d -p 8080:80 --name web -v /home/jordiop/Documents/nginx/site-content:/usr/share/nginx/html nginx`

## Resultado

![imagen](https://user-images.githubusercontent.com/95173613/168657181-e4d552dc-b9ba-4f1f-9797-dffd71c22dea.png)
