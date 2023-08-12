# Compose collection
Collection of useful (and working) docker compose files.

Currently targeting docker compose v.3.9

There are multiple ways to deploy from a compose file. Examples are provided running Docker in non-swarm mode. Feel free to use any method you see fit.
To deploy from a compose file, use this syntax from the command line.
```
docker compose -f your-compose-file.yaml up -d
```
To shut things down, use
```
docker compose -f your-compose-file.yaml down
```

Accepting PR's :)



# Repo state
## Done
* Elasticsearch single node in memory
* Elasticsearch single node with disk persistence
* Kibana stand alone
* Kibana and elasticsearch in same compose file
* Redis single node in memory
* Redis single node with disk persistence
* MSSQL standard
* MSSQL express
* Kafka stack

## Todo
* MSSQL with predefined database
* Eventstore
* RabbitMQ
* Nats / Nats-Streaming
* PostgreSQL
* FluentD

