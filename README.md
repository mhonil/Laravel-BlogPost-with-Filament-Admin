# Laravel 10 Blog Starter Kit
This is Laravel 10 blog starter kit project with [Filament PHP](https://filamentphp.com/) admin panel.




#### 1. Run `composer install`
Navigate into project folder using terminal and run

```bash
docker run --rm \
    -u "$(id -u):$(id -g)" \
    -v "$(pwd):/var/www/html" \
    -w /var/www/html \
    laravelsail/php82-composer:latest \
    composer install --ignore-platform-reqs
```

#### 2. Copy `.env.example` into `.env`

```bash
cp .env.example .env
```

#### 3. Start the project in detached mode

```bash
./vendor/bin/sail up -d
```
From now on whenever you want to run artisan command you should do this from the container. <br>
Access to the docker container
```bash
./vendor/bin/sail bash
```

#### 4. Set encryption key

```bash
php artisan key:generate --ansi
```

#### 5. Run migrations

```bash
php artisan migrate
```

#### 6. Add Filament Admin user

```bash
php artisan make:filament-user
```

## Demo
> Coming soon...

## 
