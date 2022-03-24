# Custom Dockerfile
```
# Access folder
cd nginx-example

# Build container
docker build -f Dockerfile -t bylucasxdx/nginx-example .

# Run Container
docker run --rm -d -p 80:80 bylucasxdx/nginx-example
```

# Entrypoint Example

```
cd entrypoint-example

# Build Container
docker build -f Dockerfile.entrypoint -t bylucasxdx/entrypoint .

# Run container
docker run bylucasxdx/entrypoint

# Run container changing the CMD comand
docker run bylucasxdx/entrypoint Lucas
```

# Node Example
```
cd node

# Build container
docker build -t bylucasxdx/node .

# Run container
docker run --rm -d -p 3000:3000 --name node bylucasxdx/node

# Run docker-compose
docker-compose up -d --build
```