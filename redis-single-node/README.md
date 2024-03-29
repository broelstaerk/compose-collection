# Usage
## redis-in-mem-compose.yaml
redis-in-mem-compose.yaml contans a single redis node with no disk persistence. Data will be lost when restarting the service.


```
docker compose -f redis-in-mem-compose.yaml up -d
```

## redis-persistent-compose.yaml
redis-persistent-compose.yaml contans a single redis node with disk persistence. To use this, you will need create a local volume called "redis-volume" which will be mounted in the container. Data stored in this configuration will survive restarts of the container and your local computer.

### 1. Create volume
You only need to do this once. The volume will stay there until you chose to remove it.
```
docker volume create redis-volume
```

### 2. Deploy
```
docker compose -f redis-persistent-compose.yaml up -d
```
