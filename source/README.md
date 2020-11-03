## This is where your Laravel app goes

To get started, delete this file and then do one of the following:

- Clone your project or copy all of the files directly into this `source` directory.
- Spin up the Docker network by following the instructions on the main [README.md](../README.md), and install a brand new Laravel project by running `docker-compose run --rm composer create-project laravel/laravel .` in your terminal.

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