---
description: Introduce about Docker Compose
---

# Docker Compose

### What is Compose ?&#x20;

Compose is a tool for defining and running multi-container Docker applications. With Compose you can use a `YAML` file to configure your application's services with a single command&#x20;

### YAML File

A `YAML` file of Docker Compose will look like this

```yaml
version: "3.9"
services:
  backend:
    build: .
      context: .
      dockerfile: Dockerfile
    ports:
      - "8080:8080"
    volumes:
      - log:/var/log
    network:
      - net
volumes:
  log: {}
networks:
  net:
    driver: bridge
```

### Installation

For the **Windows** and **MacOS** the Docker-Compose are already install from installer.

**Linux**

1\. Download current stable release of Docker Compose

```
mkdir -p ~/.docker/cli-plugins/
curl -SL https://github.com/docker/compose/releases/download/v2.2.2/docker-compose-linux-x86_64 -o ~/.docker/cli-plugins/docker-compose
```

2\. Apply executable permissions to the binary

```
chmod +x ~/.docker/cli-plugins/docker-compose
```

3\. Verify that Docker Compose have install successful

```
docker compose version
```
