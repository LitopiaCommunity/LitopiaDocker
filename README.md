# LitopiaDocker
Litopia docker compose env to help development and prepare production

## Nginx
### Why used reverse proxy ?
When Litopia will be deployed it will need authentification that are provide by the nestjs api, and we want to store 
the cookie of this authentification on the same adresse as the angular client

## Postgres
### Why used postgres ?
We use postgres in Litopia application to store player information. When the docker-compose.yml will be load,
it will automatically create the needed database.

## Usage
To use this docker file you first need to install docker. After that you will create `.env` file base from `.env.exemple` file.

Then edite the `.env` file with your current settings. (follow file comment to help you configure) 

Then run `docker-compose up -d` in this directory. If you get any errors

you can check it out using this command `docker-compose logs -f`