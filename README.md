# This is a laravel app deployed in docker

## Prerequisites
* Php >= 7.3
* composer
* Laravel 6.x
* docker

## Steps
1. `git clone https://github.com/DrissBoumlik/laravel_docker.git`
2. `cd laravel_docker`
3. `docker-compose build`
4. `docker-compose up -d`
5. `cd src`
6. `composer install`
7. `cp .env.example .env`
8. `php artisan key:generate`
9. `php artisan serve`
10. visit http://localhost:8088/