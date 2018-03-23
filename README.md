# Docpy
#### A minimal docker python setup with pip dependency installation. The image will automatically install dependencies from `requirements.txt` when building.

## How to Use
 - Download the repository
 - Edit the contents of `script.py` with your python script
 - Add your dependencies to `requirements.txt`
 - `$ docker-compose up`

## Adding New Dependencies
 - `$ docker-compose run python bash`
 - `$ pip install [dependency]`
 - `$ pip freeze > requirements.txt`
 - `$ exit`
 - Dependencies will be saved for the next time the script is ran

## Cleaning Up
The container will exit after the script has finished running. You can remove it either with `docker rm [container id]` or `docker-compose down -v`.
