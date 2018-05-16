# docker-lnmp

Docker files to setup Linux + Nginx + MySQL + PHP Environment.

## Services
- `nginx:latest` on `8080`
- `php:7.2-fpm` with necessary libraries on `9000`
- `mariadb` on `33060`

## Files

        +-- apps/    # web root
        +-- db/      # MySQL data dir  
        +-- logs/    # Logs
        +-- nginx/   # Nginx configuaration files
        +-- php/     
        |   +-- Dockerfile
        +-- docker-composer.yml
        
## Usage

Install [Docker](https://docs.docker.com/install/) and [Docker Compose](https://docs.docker.com/compose/install/)

        git clone https://github.com/cwang22/docker-lnmp.git
        cd docker-lnmp
        docker-compose up -d
