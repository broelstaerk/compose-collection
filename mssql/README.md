# Usage

## mssql-express-compose.yaml

```
docker compose -f mssql-express-compose.yaml up -d
```


## mssql-express-persistent-compose.yaml
mssql-express-persistence-compose.yaml contans a single mssql node with disk persistence. To use this, you will need create a local volume called "mssql-volume" which will be mounted in the container. Data stored in this configuration will survive restarts of the container and your local computer.

### 1. Create volume
You only need to do this once. The volume will stay there until you chose to remove it.
```
docker volume create mssql-volume
```

### 2. Deploy
```
docker compose -f mssql-express-persistent-compose.yaml up -d
```