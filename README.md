# How to run reviews service

```bash
/opt/ibm/wlp/bin/server run defaultServer
```

## How to run with Docker

```bash
# Build Docker Image for reviews service
docker build -t reviews .

# Run details service on port 8082
docker run -d -it --name reviews -p 8082:9080 -e ENABLE_RATINGS=true reviews
```
