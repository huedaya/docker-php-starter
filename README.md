# Docker Compose PHP Starter
Will automatically set up this following packages:
- PHP
- MariaDb
- Composer

## How to run
Make sure you're already installed Docker and Docker Compose
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
http://localhost:8080/