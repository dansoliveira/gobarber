# GoBarber API

GoBarber is an application to manage a baber shop. This repository contains the API, responsible for all business rules.
Developed on [second challenge](https://github.com/Rocketseat/bootcamp-gostack-desafio-02/blob/master/README.md#desafio-02-iniciando-aplica%C3%A7%C3%A3o) at **[Rocketseat](https://rocketseat.com.br/) Bootcamp GoStack 8.0** :rocket:.
This application will be used for personal learning, where I'll apply concepts acquired during GoStack.

# Requirements
This list contains all technologies used in development of this application. Feel free to use any other.
- For database, I use **PostgreSQL** image for [Docker](https://docs.docker.com/install/).
- **Yarn** for package management.

# Getting started
## Docker and PostgreSQL
- After install and configure Docker, run the following command on your terminal:

```
docker run --name [container_name] -e POSTGRES_PASSWORD=[db_password] -p 5432:5432 -d postgres
```

This command configure an image of PostgreSQL with `[container_name]` and `[db_password]`, on `5432` port (local machine and Docker, respectively). If all goes well, the container will start automatically after the process completes.

- Short cheatsheet ever
```shell
docker ps # list all running containers
docker ps -a # list all available containers (even if not running)
docker stop # stops the container
docker start [container_name] # starts the container
docker logs [container_name] # shows container log
```

## Config files
Replace the following words with their respective data.

### src/config/auth.js
- **YOUR_SECRET_HERE** - Secret used to encrypt/decrypt user password. Think of a random phrase, put it in [ [MD5 Online](https://www.md5online.org/), click on **Crypt** and put the generated code at this property;
- **EXPIRE_DATE** - the token expiration time. Generally, and the value used here is ** 7d ** (seven days).

### src/config/database.js

- **DIALECT_HERE** - depends of your database. In this project, the dialect is **postgres**;
- **HOST_HERE** - IP of your host. E.g. **localhost**;
- **DB_USERNAME_HERE** - your database username;
- **DB_PASSWORD_HERE** - your database password;
- **DB_NAME_HERE** - your database name. In this project, the name is **gobarber**.

## Yarn
After install Yarn, run the following commands on your terminal:
```
yarn
# await proceess completes...
yarn dev
# enjoy application
```

Feel free to contribute ;)
