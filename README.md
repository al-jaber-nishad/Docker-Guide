# Docker-Guide

This document provides a list of frequently used Docker commands to help you work with containers and images effectively.

## Basic Commands

1. **Run a Container from an Image:**
   ```bash
   docker run <image_name>
   ```

2. **List Running Containers:**
   ```bash
   docker ps
   ```

3. **List All Containers (including stopped ones):**
   ```bash
   docker ps -a
   ```

4. **Stop a Running Container:**
   ```bash
   docker stop <container_id>
   ```

5. **Remove a Container:**
   ```bash
   docker rm <container_id>
   ```

6. **List Docker Images:**
   ```bash
   docker images
   ```

7. **Remove Docker Image:**
   ```bash
   docker rmi <image_name>
   ```

## Advanced Commands

1. **Run a Container in Detached Mode (Background):**
   ```bash
   docker run -d <image_name>
   ```

2. **Map Container Port to Host Port:**
   ```bash
   docker run -p <host_port>:<container_port> <image_name>
   ```

3. **Run Interactive Shell in a Container:**
    ```bash
    docker exec -it <container_id> /bin/bash
    ```

4. **View Container Logs:**
    ```bash
    docker logs <container_id>
    ```

5. **Inspect Container Details:**
    ```bash
    docker inspect <container_id>
    ```

6. **Build a Docker Image from a Dockerfile:**
    ```bash
    docker build -t <image_name> <path_to_Dockerfile_directory>
    ```

7. **Push Docker Image to Registry (e.g., Docker Hub):**
    ```bash
    docker push <image_name>
    ```

8. **Pull Docker Image from Registry:**
    ```bash
    docker pull <image_name>
    ```

## Cleaning Up

9. **Remove All Stopped Containers:**
    ```bash
    docker container prune
    ```

10. **Remove All Unused Images:**
    ```bash
    docker image prune
    ```

18. **Remove All Containers and Images (Use with Caution!):**
    ```bash
    docker system prune -a
    ```

Remember to replace `<image_name>`, `<container_id>`, `<host_port>`, and `<container_port>` with actual values as needed.
