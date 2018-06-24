## Build Web Server Image
```sh
docker build -t voting-app:1.0 ./node/
```

## Run Web Server
```sh
docker container run --name voting-instance --rm -p 80:8888 -v ~/Projects/tryDocker/NodePostgres/node/src/:/usr/voting-app/src/  voting-app:1.0
```

## Build Database Image
```sh
docker build -t node-db:latest ./postgres/
```

## Run Database
```sh
docker container run --name node-db -p 5433:5432 --rm -v ~/Projects/tryDocker/NodePostgres/postgres/data/:/var/lib/postgresql/data/ node-db:latest
```
