docker login - must be hub.docker.com

## start

# docker container prune - remove all containers

---

Dockerfile - need read instrictions !!!

from Ubuntu

### docker-machine ip default - What ip docker

### sudo docker rm -v $(sudo docker ps -aq -f status=exited)

sudo docker run -it -h testServer --name testS -v $(pwd)/obmen:/home/obmen/ ubuntu bash

## Create new image docker

1.docker run -it --name "name" --hostname 'name' ubuntu bash

2. docker commit 'name container' 'name.hub.docker.com/nameApp'

## step - create with Dockerfile

docker build -t "name/name.image" . - dot

---

# text run docker psql

docker run -d --rm --name some-postgres \  INT ✘
-e POSTGRES_PASSWORD=2611Server \
-e PGDATA=/var/lib/postgresql/data/pgdata \
-v /home/rusdev/Projects/Podelki/post:/var/lib/postgresql/data \
-p 50432:5432 \
postgres

---

## docker-compose - file docker-compose.yml
