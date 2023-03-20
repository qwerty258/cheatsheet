docker
======

Build image

```sh
docker image build --tag name:tag --no-cache .
```

List image

```sh
docker image ls
```

Push to registry

```sh
docker image push name:tag
```

Run docker

```sh
docker container run -d name web -p 8080:8080 name:tag
```

Start/Stop docker container

```sh
docker container stop web
docker container start web
```

Remove docker container

```sh
docker container rm web
```

List container

```sh
docker container ls
```

Show docker containers

```sh
docker ps -a
```

`docker-compose`:

```sh
docker-compose build
docker-compose up
docker—compose up —d —-no—deps [service]
docker-compose down

docker-compose ps
docker-compose stop
docker-compose start
docker-compose rm
```

Log

```sh
docker-compose logs
docker-compose logs --follow
docker-compose logs --tail=5
docker-compose logs [service ...]
```

Shell into a container

```sh
docker exec -it <containerId> sh
docker-compose exec <serviceName> <shell>
```

Scale container

```sh
docker-compose up -d --scale api=4
```
