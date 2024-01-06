# Usage
## nats-in-mem-compose.yaml
nats-in-mem-compose.yaml contans a single nats node with no disk persistence. Data will be lost when restarting the service.


```
docker compose -f nats-in-mem-compose.yaml up -d
```
