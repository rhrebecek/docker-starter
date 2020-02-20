# Docker Starter

- [Presentation](/docs/presentation.pdf)

## Authors
- [Radek Hřebeček](https://hrebecek.cz)

## Before starting the project
- [Install Docker engine](https://docs.docker.com/install/linux/docker-ce/ubuntu)
- [Install Docker compose](https://docs.docker.com/compose/install)

## How to start
1. Run containers in docker `docker-compose up --build`
2. Go to website `http://localhost:8000`

## Commands
- `docker-compose exec php /bin/bash` connect to PHP container for work
- `docker-compose run --rm node install --save react react-dom` instal dependencies for NPM project
- `docker-compose stop` for end work
- `docker system prune -a` all remove containers and images, networks, volumes
