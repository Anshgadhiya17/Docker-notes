# 📘 Dockerfile

A Dockerfile is a script containing instructions to build a Docker image.

---

## Basic Dockerfile Example

```dockerfile
FROM node:18
WORKDIR /app
COPY package.json .
RUN npm install
COPY . .
EXPOSE 3000
CMD ["npm", "start"]
```

---

## Common Instructions

- FROM → Base image
- WORKDIR → Set working directory
- COPY → Copy files
- RUN → Execute command
- EXPOSE → Open port
- CMD → Run application

---

## Build Image

```bash
docker build -t myapp .
```

---
