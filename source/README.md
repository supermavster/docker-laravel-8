# This is where your Laravel app goes

Add your Laravel project here (or create a new blank one).

**Note:** IF exist problems generate the project delete this README.md

---

## Help

A little help to create the project:

### Make a new Project

```sh
docker-compose run --rm composer create-project laravel/laravel .
```

### Copy Environment

```sh
cp .env.example .env
```

---

### Install Libraries from Composer

```sh
docker-compose run --rm composer install
```

### Install Libraries from Node

```sh
docker-compose run --rm npm install
```

### Clear/Clean the project

```sh
docker-compose run --rm artisan clear:data
docker-compose run --rm artisan cache:clear
docker-compose run --rm artisan view:clear
docker-compose run --rm artisan route:clear
docker-compose run --rm artisan clear-compiled
docker-compose run --rm artisan config:cache
docker-compose run --rm artisan storage:link
```

### Generate Keys

```sh
docker-compose run --rm artisan key:generate
```

### Run migrations

```sh
docker-compose run --rm artisan migrate --seed
```

### Run Passport (Optional)

```sh
docker-compose run --rm artisan passport:install
```
