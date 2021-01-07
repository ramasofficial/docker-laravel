# Installation
Upload /docker folder and docker-compose.yml to your project root laravel directory.

Copy .env.example to .env or change it for your .env file if not exists this parameters.

# Description
All you need for default laravel server stack with Docker.

- Laravel 8, but i think works and with Laravel 7
- PHP 8.0
- MYSQL 5.7
- Phpmyadmin

# Configure docker in server

If your server is ubuntu all commands starts with sudo command before.

Example: sudo docker-compose ...

# Build docker images

Build docker images:
```
sudo docker-compose build --no-cache
```

Start all containers:
```
sudo docker-compose up -d
```

Stops all containers:
```
sudo docker-compose down
```

Stops all containers and delete mysql volume data:
```
sudo docker-compose down -v
```

# Shows all working containers
```
sudo docker ps
```

# Execute actions

Execute composer update command:
```
sudo docker-compose exec app composer update
```

Execute artisan key generate:
```
sudo docker-compose exec app php artisan key:generate
```

Execute database migrate:
```
sudo docker-compose exec app php artisan migrate
```
