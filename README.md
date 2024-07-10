# self-dash-backend

this repository is backend

using base project or study etc

- laravel 11
- MySQL 8.0
- nginx

## addon vscode plugin

- Remote Development
- Laravel Blade Snippets

## Getting Start

- settings docker-cmpose.yml

  - change to your mysql db password and user etc setting

- nginx conf settings

  - change the settings to your project name
  - pilic dir etc

- next container build and up

  - `$ docker-compose build`
  - `$ docker-compose up`

- next exec container and create laravel project
  - `$ docker-compose exec app bash`
  - `$ composer create-project --prefer-dist laravel/laravel self-dash-backend "11.*"`
  - `$ chown www-data storage/ -R`

## laravel

- change `.env` DB_XXXX etc...

```
DB_CONNECTION=
DB_HOST=
DB_PORT=
DB_DATABASE=
DB_USERNAME=
DB_PASSWORD=
```

- URL:http://localhost:8000/

## admin

- http://localhost:8080/

### How to artisan

- migrate:`https://readouble.com/laravel/11.x/ja/migrations.html`
  - `php artisan migrate`
  - `php artisan migrate:rollback --step={number|*}`
