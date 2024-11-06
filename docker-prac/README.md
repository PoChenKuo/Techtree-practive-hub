# Docker Practice (docker-prac)

## Overview

The **docker-prac** project is part of the **Techtree Practice Hub** and serves as a focused environment for learning and practicing Docker. This project aims to help you gain hands-on experience with Docker by building and running containerized applications.

### Goals

1. **Understand Docker Basics**: Learn how to create Docker images, run containers, and work with Dockerfiles.
2. **Multi-Service Docker Setup**: Use Docker Compose to manage a multi-container environment, involving a frontend, backend, database, and cache.
3. **Build an Example Application**: Practice building an example application using React, Django, MySQL, and Redis, all running in Docker containers.

## Project Structure
docker-prac/
├── README.md               # Project overview and guide
├── Tutorial.md             # Step-by-step Docker tutorial
├── Task.md                 # Instructions for building and running the example application
├── frontend/               # React frontend application
│   ├── Dockerfile
│   └── ...                 # Other files related to the frontend
├── backend/                # Django backend application
│   ├── Dockerfile
│   ├── requirements.txt
│   └── ...                 # Other files related to the backend
├── docker-compose.yml      # Docker Compose file to manage multi-container setup
└── init.sql                # SQL script to initialize MySQL database

- **frontend/**: Contains the Docker configuration and code for the React frontend application.
- **backend/**: Contains the Docker configuration, requirements, and code for the Django backend application.
- **docker-compose.yml**: Defines and manages the multi-service setup, including the React frontend, Django backend, MySQL database, and Redis cache.
- **init.sql**: Initializes the MySQL database with necessary tables and users.

## Getting Started

1. **Tutorial**: Refer to `Tutorial.md` for a detailed guide on Docker basics and setting up containers.
2. **Build and Run the Example**: Follow `Task.md` for instructions on building and running the example application using Docker and Docker Compose.

## Usage

To start the project, use Docker Compose:

```bash
docker-compose up --build
```
