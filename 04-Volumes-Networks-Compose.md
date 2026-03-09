# 📘 Volumes, Networks & Docker Compose

---

## Volumes

Used to persist data.

```bash
docker volume create myvolume
```

Attach volume:
```bash
docker run -v myvolume:/data imageName
```

---

## Networks

Used for container communication.

```bash
docker network create mynetwork
```

---

## Docker Compose

Used to run multiple containers using a YAML file.

Example `docker-compose.yml`:

```yaml
version: '3'
services:
  app:
    image: node
    ports:
      - "3000:3000"
```

Run:
```bash
docker-compose up
```

---
