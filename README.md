# Go Web App

A simple Golang web application that returns "Hello World." when accessed.

## Features

- Simple HTTP server on port 8080
- Returns "Hello World." message
- Dockerized for easy deployment
- Multi-stage Docker build for optimized image size

## Running Locally

### Option 1: Using Go directly

```bash
go run main.go
```

The server will start on `http://localhost:8080`

### Option 2: Using Docker

1. Build the Docker image:
```bash
docker build -t go-web .
```

2. Run the container:
```bash
docker run -p 8080:8080 go-web
```

The server will be available at `http://localhost:8080`

## Testing

You can test the application by visiting `http://localhost:8080` in your browser or using curl:

```bash
curl http://localhost:8080
```

Expected response: `Hello World.`