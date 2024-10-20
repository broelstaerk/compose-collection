# Usage

## openvpn-server-compose.yaml
A stack consisting of single openvpn server.

### 1. Create volumes
You only need to do this once. The volume will stay there until you chose to remove it.
```
docker volume create openvpn-volume
```

### 2. Deploy
```
docker compose -f openvpn-server-compose.yaml up -d
```