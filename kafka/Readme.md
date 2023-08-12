# Usage

## kafkastack-compose.yaml

```
docker compose -f kafkaastack-compose.yaml up -d
```
The kafkastack-compose.yaml is a stack consisting of:
- Kafka message broker 
- Schema registry (https://github.com/confluentinc/schema-registry)
- Zoo keeper 
- Control center (https://github.com/confluentinc/control-center-images - subject to confluent enterprise license)  
- Rest proxy (https://github.com/confluentinc/kafka-rest)

Once up, you can access the control center at http://[IpAddress]:9021

## License info
All images in this stack is based on images from Confluent Inc. Please consult their license information before using. Read all about it here: https://docs.confluent.io/platform/current/installation/docker/image-reference.html
