# Usage
## redis-in-mem-compose.yaml
redis-in-mem-compose.yaml contans a single redis node with no disk persistence. Data will be lost when restarting the service.


```
docker stack deploy --compose-file redis-in-mem-compose.yaml redis-in-mem
```

## redis-persistence-compose.yaml
redis-persistence-compose.yaml contans a single redis node with disk persistence. To use this, you will need to map a local folder which can be mounted to the container. Data stored in this configuration will survive restarts of the container.


```
docker stack deploy --compose-file redis-persistent-compose.yaml redis-persistent
```
