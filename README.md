# WordPress Docker Compose
wordpress, mysql, phpmyadmin, nginx, docker-compose

An easy way WordPress development with Docker Compose.

## Requirements
Make sure you have **Docker** and **Docker Compose** installed on your machine.

## Configuration
### 1,First, write your .env file like [example.env](https://github.com/MohammadrezaJavid/wordpress-and-mysql-docker-compose/blob/master/example.env)
### 2, Register your desired domain in two files([nginx.conf](https://github.com/MohammadrezaJavid/wordpress-and-mysql-docker-compose/blob/67f6b38c7ddf25faee50cd3395e22f3a4e768044/nginx-config/nginx.conf#L5) and [docker-compose.yml](https://github.com/MohammadrezaJavid/wordpress-and-mysql-docker-compose/blob/67f6b38c7ddf25faee50cd3395e22f3a4e768044/docker-compose.yml#L80))

## Installation

Open a terminal and cd into the folder containing docker-compose.yml and run the following command:

### 1, Pull the required images:

```
docker-compose pull
```

### 2, Launching containers:

```
docker-compose up -d
```

### 3, And now refer to the domain that you have registered in these two files([nginx.conf](https://github.com/MohammadrezaJavid/wordpress-and-mysql-docker-compose/blob/67f6b38c7ddf25faee50cd3395e22f3a4e768044/nginx-config/nginx.conf#L5) and [docker-compose.yml](https://github.com/MohammadrezaJavid/wordpress-and-mysql-docker-compose/blob/67f6b38c7ddf25faee50cd3395e22f3a4e768044/docker-compose.yml#L80)) so that the main page of wordpress can be seen.

## Usage
### Stop or start containers
```
docker-compose stop
```
```
docker-compose start
```

## Removing containers
### Stop and remove all containers:
```
docker-compose down
```
### and use `-v` if you need to remove all volumes and networks bridge:
```
docker-compose down -v
```
### PhpMyAdmin
You can also visit `http://yourdomain:8080` to access phpMyAdmin after starting the containers.
