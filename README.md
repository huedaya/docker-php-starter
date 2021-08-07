# Docker Compose PHP Starter
Automatically set up this following packages:
- PHP
- MariaDb
- Composer

## How to run
Make sure you're already installed [Docker](https://docs.docker.com/get-docker/) and [Docker Compose](https://docs.docker.com/compose/install/)
```bash
cp .env.example .env
docker compose up -d
docker-compose exec app bash
```

Then, inside container 
```bash
composer run app-init
```

## Enjoy
[http://localhost:8080/](http://localhost:8080/)