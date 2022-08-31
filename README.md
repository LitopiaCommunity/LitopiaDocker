# LitopiaDocker
Litopia docker compose env to help devloppement and prepare production

## Why used reverse proxy ?
When litopia will be deploy it will need authentification that are provide by the nestjs api and we want to store 
the cookie of this authentification on the same adresse as the angular client

## Usage
To use this docker file you first need to install docker. After that you will create `.env` file base from `.env.exemple` file.

Then edite the `.env` file with your current settings. (follow file comment to help you configure) 

Then run `docker-compose up -d` in this directory. If you get any errors

you can check it out using this command `docker-compose logs -f`