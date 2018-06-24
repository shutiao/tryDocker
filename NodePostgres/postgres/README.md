## Find IP address of database which node-app is going to connected to
IPAM/Config/Gateway   
```sh
docker inspect network bridge
```

## Postgres Client Connection
```sh
docker container exec -it node-db psql -U postgres
```

## Display Table
```sh
\dt
```

## List Database
```sh
\l
```
