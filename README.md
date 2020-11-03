# Docker - Laravel

![Docker](https://github.com/supermavster/docker-laravel-8/workflows/Docker/badge.svg)

![](https://repository-images.githubusercontent.com/309769351/1c0dfc80-1def-11eb-9e5c-641da3e3c9b4)

A pretty simplified Docker Compose workflow that sets up a LEMP network of containers for local Laravel development.

## Ports

- **nginx** - `:8080`
- **mysql** - `:3306`
- **php** - `:9000`
  - with **xdebug** - `:9001`
- **redis** - `:6379`
- **phpmyadmin** - `:8081`

## Use

- `docker-compose up --build`
- `docker-compose down -v`

## Special Cases

- `docker-compose run --rm composer update`
- `docker-compose run --rm npm run dev`
- `docker-compose run --rm artisan migrate` 
