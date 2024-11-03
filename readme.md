# Nginx Docker Boilerplate

A simple boilerplate for running Nginx in a Docker container. This setup includes a customizable `nginx.conf` file for redirecting requests to local applications, making it ideal for local development environments.

## Features

- **Docker Compose**: Easily deploy Nginx using Docker Compose.
- **Proxy Configuration**: Forward requests to services running on your host machine (default to port 3000).
- **Resource Limits**: Configured with CPU and memory limits for efficient resource management.
- **Automatic Restart**: The Nginx container will restart automatically to ensure high availability during development.

## Quick Start

1. **Clone the Repository**:
  ```bash
   git clone https://github.com/rajraii/nginx-docker-boilerplate.git
   
   cd nginx-docker-boilerplate
  ```

2. **Customize Nginx Configuration**:
  Edit the nginx.conf file to adjust proxy settings for your applications. The default configuration proxies requests to 
  `http://host.docker.internal:3000`.

3. **Run Docker Compose**
  ```bash
    docker-compose up
  ```