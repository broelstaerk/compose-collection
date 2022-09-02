# Compose collection
Collection of useful (and working) docker compose files.

Currently targeting docker compose v.3.9

There are multiple ways to deploy from a compose file. Exmaples are provided running docker in non-swarm mode. Feel free to use any method you see fit.
To deploy from a compose file, use this syntax from the command line.
```
docker compose -f your-compose-file.yaml up -d
```
To shut things down, use
```
docker compose -f your-compose-file.yaml down
```

Accepting PR's :)

## To get started with docker swarm
```
docker swarm init
```

# Repo state
## Done
* Elasticsearch single node in memory
* Elasticsearch single node with disk persistence
* Kibana stand alone
* Kibana and elasticsearch in same compose file
* Redis single node in memory
* Redis single node with disk persistence

## Todo
* MSSQL standard
* MSSQL with predefined database
* Eventstore
* Kafka
* RabbitMQ
* Nats / Nats-Streaming
* PostgreSQL
* FluentD

