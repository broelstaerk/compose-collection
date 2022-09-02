# Usage

## kibana-standalone-compose.yaml
Kibana as a standalone application does not make much sense. You probably want to spin up a elasticsearch container before starting kibana.

This example is dependent on having access to an elasticsearch instance via the DNS name "elasticssearch". The elasticsearch compose examples are configured to work together with this kibana configuation.

```
docker compose -f kibana-standalone-compose.yaml up -d
```

## kibana-elasticsearch-compose.yaml
Starts a elasticsearch instance without disk persistence (your data will be lost when elasticsearch shuts down or restarts) and a kibana container.

```
docker compose -f kibana-elasticsearch-compose.yaml down
```