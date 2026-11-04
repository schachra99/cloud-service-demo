# Cloud Service Demo

## Project Name
Cloud Service Demo

## Project Purpose
The purpose of this project is to create a simple sample web application that represents a service that could be hosted on a cloud platform.

## Files Included
- **README.md:** Provides information about the project, its purpose, and the files included.
- **index.html:** Contains the HTML code for the sample Cloud Service Demo webpage.

## How Version Control Helps a Cloud Project
Version control helps a cloud project by tracking changes, maintaining a history of updates, allowing team members to collaborate, and making it easier to restore previous versions when needed. ## Docker and Containerization

### What is Docker?

Docker is a platform that allows applications to run in isolated environments called containers. It helps applications run consistently across different computers and environments.

### What is a Docker Image?

A Docker image is a packaged template that contains the application and the instructions needed to create a container.

### What is a Docker Container?

A Docker container is a running instance created from a Docker image. It provides an isolated environment in which the application can run.

### Building the Docker Image

To build the Docker image, run:

```bash
docker build -t cloud-service-demo:1.0 .
```

### Running the Docker Container

To start the application inside a container, run:

```bash
docker run -d --name cloud-demo-container -p 8080:80 cloud-service-demo:1.0
```

### Accessing the Application

Open the following address in a web browser:

`http://localhost:8080`

### Docker Configuration

The project includes a Dockerfile that uses the lightweight Nginx Alpine image to serve the index.html webpage.

Docker helps cloud projects by packaging applications into portable containers that can run consistently across different environments.