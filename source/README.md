## This is where your Laravel app goes

To get started, make sure you have [Docker installed](https://docs.docker.com/) on your system, and then clone this repository.

Follow the next steps:

1. Navigate in your terminal to the directory you cloned this.
2. Run `cp .env.example .env` and configure your database credentials to the .env file 
3. Spin up the containers for the web server by running `docker-compose up -d --build site`.

After that completes, follow the steps from the [source/README.md](README.md) file to get your Laravel project added in (or create a new blank one).


--- 

A little help to create the project: 

```sh
# Make a new Project
docker-compose run --rm composer create-project laravel/laravel .

# Copy Environment
cp .env.example .env 

# Install Libraries from Composer
docker-compose run --rm composer install 

# Install Libraries from Node
docker-compose run --rm npm install 

# Clear/Clean the project
docker-compose run --rm artisan clear:data
docker-compose run --rm artisan cache:clear 
docker-compose run --rm artisan view:clear 
docker-compose run --rm artisan route:clear 
docker-compose run --rm artisan clear-compiled 
docker-compose run --rm artisan config:cache
docker-compose run --rm artisan storage:link

# Generate Keys
docker-compose run --rm artisan key:generate

# Run migrations
docker-compose run --rm artisan migrate --seed

# Run Passport (Optional)
docker-compose run --rm artisan passport:install
```
