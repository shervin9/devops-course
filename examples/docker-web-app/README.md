# Docker Web App Example

A simple Node.js web application containerized with Docker, demonstrating basic Docker concepts covered in Module 4.

## Project Structure

```
docker-web-app/
├── Dockerfile
├── docker-compose.yml
├── src/
│   ├── index.js
│   ├── package.json
│   └── public/
│       ├── index.html
│       └── style.css
└── README.md
```

## Prerequisites

- Docker installed on your machine
- Docker Compose installed on your machine
- Basic understanding of Node.js

## Building and Running with Docker

### Option 1: Using Docker directly

1. Build the Docker image:
   ```bash
   docker build -t docker-web-app .
   ```

2. Run the Docker container:
   ```bash
   docker run -p 3000:3000 docker-web-app
   ```

3. Access the application in your browser at http://localhost:3000

### Option 2: Using Docker Compose

1. Start the application using Docker Compose:
   ```bash
   docker-compose up
   ```

2. Access the application in your browser at http://localhost:3000

## Features Demonstrated

- Dockerfile creation and best practices
- Container port mapping
- Volume mounting for development
- Environment variable usage
- Docker Compose for multi-container setup

## Further Learning

- Try modifying the application and observe how the changes are reflected
- Add a database container to the Docker Compose file
- Implement a production-ready Nginx configuration
- Set up a CI/CD pipeline for the application 