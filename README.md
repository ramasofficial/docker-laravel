# Installation
Upload /docker folder and docker-compose.yml to your project root laravel directory.

Copy .env.example to .env or change it for your .env file if not exists this parameters.

# Info
All you need for laravel.
Docker, laravel 8, php 8, mysql, phpmyadmin

# Configure in server

If your server is ubuntu with docker all commands start with sudo command.

Example: sudo docker-compose ...

# Build docker images
```
sudo docker-compose build - Build docker images
```

```
sudo docker-compose up -d - Start all containers
```

```
sudo docker-compose down - Stops all containers
```

```
sudo docker-compose down -v - Stops all containers and delete mysql volume
```

# Shows all working containers

```
sudo docker ps - Showing all working containers
```

# Execute actions

```
sudo docker-compose exec app composer update - Execute composer update command
```

```
sudo docker-compose exec app php artisan key:generate - Execute artisan key generate
```

```
sudo docker-compose exec app php artisan migrate - Execute database migrate
```
