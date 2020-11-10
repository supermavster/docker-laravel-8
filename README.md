# Docker - Laravel

![Docker](https://github.com/supermavster/docker-laravel-8/workflows/Docker/badge.svg)

![Image](https://repository-images.githubusercontent.com/309769351/1c0dfc80-1def-11eb-9e5c-641da3e3c9b4)

A pretty simplified Docker Compose workflow that sets up a LEMP network of containers for local Laravel development.

## Ports

Ports used in the project:
| Software  | Port   |
|-------------- | -------------- | -------------- |
| **nginx**    | 8080     |
| **phpmyadmin**    | 8081     |
| **mysql**    | 3306     |
| **php**    | 9000     |
| **xdebug**    | 9001     |
| **redis**    | 6379     |


## Use

1. Generate your own `.env` to docker compose with the next command:

    ```sh
      cp .env.example .env
    ```

2. Create or Put your laravel project in the folder source; to create follow the next instructions [Here](source/README.md).
3. Build the project whit the next commands:

    ```sh
    docker-compose up --build
    ```

**Note:** To Down and remove the volumes we use the next command:

```sh
docker-compose down -v
```

## Special Cases

Update Composer:

```sh
docker-compose run --rm composer update
```

Run compiler (Webpack.mix.js) or Show the view compiler in node:

```sh
docker-compose run --rm npm run dev
```

Run all migrations:

```sh
docker-compose run --rm artisan migrate
```
