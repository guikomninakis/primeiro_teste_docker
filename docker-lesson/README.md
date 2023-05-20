## Rodando

Com docker

1. `docker build -t docker-lesson`
2. `docker run -p 5173:5173 docker-lesson`

OBS: Precisamos do -p pois fazemos o mapeamento da porta do container para a porta do Docker host (nossa maquina!), referência:

> https://docs.docker.com/config/containers/container-networking/

### Como debugar a sua imagem Docker

As vezes precisamos entrar no Container para executar uns comandos e ver como ficou o codigo la dentro.

Precisamos primeiro, pegar o Docker Container ID:

`docker ps`

Com o container id, executamos:

`docker exec -it {{docker-container-id}} sh`

E estaremos dentro do Container.

