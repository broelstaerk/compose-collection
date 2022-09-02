# Usage
## elasticsearch-in-mem-compose.yaml
elasticsearch-in-mem-compose.yaml contans a single elasticsearch node with no disk persistence. Data will be lost when restarting the service.


```
docker compose -f elasticsearch-in-mem-compose.yaml up -d
```

## elasticsearch-persistence-compose.yaml
elasticsearch-persistence-compose.yaml contans a single elasticsearch node with disk persistence. To use this, you will need create a local volume called "elasticsearch-volume" which will be mounted in the container. Data stored in this configuration will survive restarts of the container and your local computer.

### 1. Create volume
You only need to do this once. The volume will stay there until you chose to remove it.
```
docker volume create elasticsearch-volume
```

### 2. Deploy
```
docker compose -f elasticsearch-persistent-compose.yaml down
```

