# Docker First Project — Custom Nginx Website

My first hands-on Docker project. This project packages a custom HTML webpage into a Docker image using Nginx and runs it inside a container.

## Technologies Used

- Ubuntu Linux
- Docker
- Nginx
- HTML
- Git and GitHub

## Project Structure

```text
docker-first-project/
├── Dockerfile
├── index.html
└── README.md
```

## Build the Docker Image

Clone this repository and enter the project directory, then run:

```bash
sudo docker build -t taaha-docker-website:v1 .
```

## Run the Container

```bash
sudo docker run -d --name taaha-website -p 8081:80 taaha-docker-website:v1
```

Open `http://localhost:8081` in your browser to view the website.

## Container Management

Check running containers:

```bash
sudo docker ps
```

Stop the container:

```bash
sudo docker stop taaha-website
```

Start it again:

```bash
sudo docker start taaha-website
```

## Docker Hub

The published image is available here:

https://hub.docker.com/r/taahadockerr/taaha-docker-website

Pull the image:

```bash
sudo docker pull taahadockerr/taaha-docker-website:v1
```

## What I Learned

- Creating a Dockerfile
- Building a custom Docker image
- Running and managing containers
- Mapping host ports to container ports
- Publishing a Docker image to Docker Hub
- Managing source code with Git and GitHub

## Author

Taaha Mustafa Khan

GitHub: https://github.com/taahakhan-stack
