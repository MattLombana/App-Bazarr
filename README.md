# App-Bazarr

## First Time Prerequisites

1. Run [Traefik](https://github.com/HackingServerHomelab/App-Traefik)

## Running the Containers

1. Update the following lines in [docker-compose.yml](./Docker/docker-compose.yml)
    * `../Data/config:/config`
    * `../Data/movies:/movies`
    * `../Data/tv:/tv`
2. Update the Traefik host label in [docker-compose.yml](./Docker/docker-compose.yml)
    * ``"traefik.http.routers.bazarr.rule=Host(`localhost`)"``
3. Run `docker-compose -f ./Docker/docker-compose.yml up -d`

## First Time Setup

1. Visit <https://your-ip>
