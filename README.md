# docker

Ambiente de teste Arch linux

## Instalando docker
yaourt -S docker


Adcionando a o grupo para exercutar toda hora sudo

$ gpasswd -a USUARIo dockeR


## Usando o Docker

* Listando images

$ docker images

* Procurando images

$ docker seach debian

* Baixando images

$ docker pull debian

* Listando contener rodando
$ docker ps 

## Levantando um coteiner

* Levantando uma image
$ docker run -ti ubuntu bash

Voce pode pausar e sair do coteiner com o crtl+p e crtl+q

* Voltando para o coteiner
$ docker exec -ti ID 

Ou 

$ docker attach ID bash

## Salvando uma imagem
$ docker commit ID USER/app:TAG


## Excluindo uma imagem
Para excluir a imagem você deve escluir primeiro coteiner
$ docker ps -a

Removendo coteiner:

$ docker rm ID

Removendo imagem:

$ docker rmi ID
