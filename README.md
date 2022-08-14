# Project name

Short description here.

## Components

Name | Purpose
---|---
Python | Flask app
Postgres | Database
Caddy | SSL with LetsEncrypt
Adminer | Database admin (only for development)

## Usage
- Install [Debian 11](https://www.debian.org/releases/stable/)
- Install [Docker](https://docs.docker.com/engine/install/debian/#install-using-the-repository) and Git from repositories
- Clone this repository.
- Copy `.env-example` to `.env` and fill in

## Run
### Development
```
docker-compose -f docker-compose.yml -f docker-compose-development.yml up
```
### Production with HTTPS/SSL by LetsEncrypt
```
docker-compose -f docker-compose.yml -f docker-compose-ssl.yml up
```
