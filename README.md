# VLMCSD for Docker

Deploy vlmcsd service on Docker container

```bash
git clone https://github.com/Wind4/vlmcsd-docker.git vlmcsd
cd vlmcsd

# Use docker-compose service
docker-compose up -d

# or docker build image
docker build -t vlmcsd .
docker run -idt -p 1688:1688 vlmcsd
```

Build multi arch
```
docker buildx build --platform linux/amd64,linux/amd64/v2,linux/amd64/v3,linux/arm64,linux/s390x,linux/386,linux/arm/v7,linux/arm/v6 -t vlmcsd:latest .

```
