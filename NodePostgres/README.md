## Run Web Server
```sh
docker container run --name voting-instance --rm -p 80:8888 -v ~/Projects/tryDocker/NodePostgres/src/:/usr/voting-app/src/  voting-app:1.0
```
## Run Database
```sh
docker container run --name node-db -p 5433:5432 --rm -v ~/Projects/tryDocker/NodePostgres/postgres/data/:/var/lib/postgresql/data/ node-db:latest
```
