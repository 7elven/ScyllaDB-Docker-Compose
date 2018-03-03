# ScyllaDB-Docker-Compose

### How to use ScyllaDB with Docker-Compose
create file docker-compose.yml include

```yaml
version: '3'
services:
  scylla:
    image: "scylladb/scylla"
    ports:
     - "9042:9042"
    volumes:
     - /var/lib/scylla:/var/lib/scylla
    restart: always
    command: '--experimental 1'
```
