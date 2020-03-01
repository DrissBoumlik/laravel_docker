# This is a laravel app deployed in docker

## Requirements
* Git
* Docker
- If you want to work with the files from your local machine you will need :
    * Php >= 7.2
    * Composer
    * Laravel 6.x

## Steps
1. `git clone https://github.com/DrissBoumlik/laravel_docker.git`
2. `cd laravel_docker`
3. `docker-compose build`
4. `docker-compose up -d`
5. `cd src`
6. `docker-compose exec php composer install -d /var/www/html`
7. `cp .env.example .env`
8. `docker-compose exec php php /var/www/html/artisan key:generate`
9. Visit http://localhost:8088
10. If you would like to change the port check docker-compose.yml nginx configuration line 11.
11. If you want to work with the database then run `docker-compose exec php php /var/www/html/artisan migrate`