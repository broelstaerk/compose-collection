# Compose collection
Collection of useful (and working) docker compose files.

Currently targeting docker compose v.3.9

Deployment examples are based on docker swarm where each compose file is launched as an individual stack. Feel free to use any deployment method you see fit.

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

