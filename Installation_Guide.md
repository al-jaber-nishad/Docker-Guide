# Docker Installation and Image Usage Guide

This guide will walk you through the process of installing Docker, pulling an image from Docker Hub, and running it on your local system.

## Table of Contents
- [Prerequisites](#prerequisites)
- [Step 1: Install Docker](#step-1-install-docker)
- [Step 2: Verify Docker Installation](#step-2-verify-docker-installation)
- [Step 3: Pull an Image from Docker Hub](#step-3-pull-an-image-from-docker-hub)
- [Step 4: Run the Docker Image](#step-4-run-the-docker-image)
- [Conclusion](#conclusion)

## Prerequisites
Before you begin, make sure you have the following prerequisites:
- A computer running a supported operating system (Linux, Windows, or macOS)
- An active internet connection

## Step 1: Install Docker

### Linux
 Easiest way to do it is using the offical script.
```bash 
curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh get-docker.sh
```

### Windows
1. Download the Docker Desktop for Windows from the [Docker website](https://www.docker.com/products/docker-desktop) and follow the installation instructions.

### macOS
1. Download Docker Desktop for Mac from the [Docker website](https://www.docker.com/products/docker-desktop) and follow the installation instructions.

## Step 2: Verify Docker Installation
To verify that Docker is installed and running, open a terminal or command prompt and run:

```bash
docker --version
```

This command should display the installed Docker version.

## Step 3: Pull an Image from Docker Hub
Docker images are available on [Docker Hub](https://hub.docker.com/), a public registry for Docker images. To pull an image from Docker Hub, use the `docker pull` command. Replace `image_name` with the name of the image you want to pull.

```bash
docker pull image_name
```

For example, if you want to pull the official Ubuntu image, you can use:

```bash
docker pull ubuntu
```

## Step 4: Run the Docker Image
Once you have pulled the image, you can run a container based on that image using the `docker run` command. Replace `image_name` with the name of the image you pulled in the previous step.

```bash
docker run -it --name my_container image_name
```

- `-it` enables an interactive terminal.
- `--name my_container` assigns a name to the running container (you can choose any name you like).
- `image_name` is the name of the Docker image.

For example, to run a basic Ubuntu container:

```bash
docker run -it --name my_ubuntu ubuntu
```

You will now be inside the Ubuntu container, and you can interact with it as if it were a separate Linux system. To exit the container, simply type `exit`.

## Conclusion
You have successfully installed Docker, pulled an image from Docker Hub, and run a Docker container on your local system. Docker makes it easy to deploy and manage containerized applications, providing an efficient and consistent development and deployment environment. Explore Docker Hub for a wide range of available images to suit your needs.
