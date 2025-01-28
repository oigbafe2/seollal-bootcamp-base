# Seollal Bootcamp Base Project

# Updated by Igbafe

This project is meant to act as a baseline for building your Seollal bootcamp project.

## Setup for Development

```shell
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -e ".[dev]"
pre-commit install
```

## Running

### For Dev

<!-- ```shell
source .venv/bin/activate  # if not done already
run
``` -->


``` shell
docker compose up -d
# this runs the image as a container named back server, deletes the container
# joins it to the network of the containers running via docker compose put
#port 80 to our port 8000 and sets the environemnt variable properly

docker run --name backend_server --rm --publish 8000:80 seoullal-bootcamp

```
