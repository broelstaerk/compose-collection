# Usage

## postgresql-pgadmin-compose.yaml
A stack consisting of postgreSQL and pgadmin. Nothing is persisted on external volumes so data and configurations will be lost when restarting containers.
```
docker compose -f postgresql-pgadmin-compose.yaml up -d
```

## postgresql-pgadmin-persistent-compose.yaml
Stack consisting of postgreSQL and pgadmin. Both are persisting data on external volumes so data will survive restarts. Remember to create volumes before starting containers.

### 1. Create volumes
You only need to do this once. The volume will stay there until you chose to remove it.
```
docker volume create postgres-volume
docker volume create pgadmin-volume
```

### 2. Deploy
```
docker compose -f postgresql-pgadmin-persistent-compose.yaml up -d
```