# Instalación y configuración Docker

*La instalación es realizada en Ubuntu*

## Comprobación y eliminación de versiones instaladas

`sudo apt-get remove docker docker-engine docker.io containerd runc`

## Preparar el repositorio

Actualizamos repositorios

`sudo apt-get update`

Instalamos algunas dependencias

```
sudo apt-get install \
>     ca-certificates \
>     curl \
>     gnupg \
>     lsb-release
```
Acabamos de preparar el repositorio

`curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg`

```
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

```

## Instalación

`sudo apt-get update`

Instalamos docker

`sudo apt-get install docker-ce docker-ce-cli containerd.io docker-compose-plugin`

## Iniciar y probar docker

`sudo docker run hello-world`

![imagen](https://user-images.githubusercontent.com/95173613/167732692-9f8779dc-d15f-4cf1-a294-e0ccfe6081c9.png)
