# Usage
## nats-in-mem-compose.yaml
nats-in-mem-compose.yaml contans a single nats node with no disk persistence. Data will be lost when restarting the service.


```
docker compose -f nats-in-mem-compose.yaml up -d
```


## nats-persistent-compose.yaml
nats-persistent-compose.yaml contans a single nats node with disk persistence. Data will be kept across restarts.

### 1. Create volume
You only need to do this once. The volume will stay there until you chose to remove it.
```
docker volume create nats
```

### 2. Deploy
```
docker compose -f nats-in-mem-compose.yaml up -d
```
