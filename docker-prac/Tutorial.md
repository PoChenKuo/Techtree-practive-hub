# Docker Tutorial

## 1. What is Docker?

Docker is a platform that allows you to develop, ship, and run applications in isolated environments called containers. Containers bundle an application with all its dependencies, making it easy to run across different environments.

## 2. Docker Basics

Images: Read-only templates that define the instructions for creating a Docker container.
Containers: Instances of Docker images that run your application.
Dockerfile: A text file with instructions for building a Docker image.
Docker Compose: A tool that allows you to define and manage multi-container Docker applications in a single YAML file.

## 3. Common Docker Commands

### Build an image:

```bash
docker build -t <image_name> .
```

### Run a container:

```bash
docker run -d -p <host_port>:<container_port> <image_name>
```

### Stop a container:

```bash
docker stop <container_id>
```

### List running containers:

```bash
docker ps
```

### Use Docker Compose:

```bash
docker-compose up
docker-compose down
```

## 4. Basic Dockerfile Structure

A Dockerfile includes instructions to set up an environment and install dependencies:

```Dockerfile
# Start from a base image
FROM python:3.9

# Set working directory
WORKDIR /app

# Copy application files
COPY . .

# Install dependencies
RUN pip install -r requirements.txt

# Define the command to run the app
CMD ["python", "app.py"]
```
