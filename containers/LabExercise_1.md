# Container Training Labs

Welcome to the Container Training Labs! In these exercises, you will learn how to use Podman to run containerized applications. Make sure you have Podman installed on your system before proceeding.

## Exercise 1: Running an Image using NGINX

#### Objective: Understand how to run a containerized NGINX web server using Podman.

1. Pull the NGINX image from Docker Hub:
   ```bash
   $ podman pull nginx
   ```
2. Start a container from the NGINX image:
   ```bas
   $ podman run --name mynginx -d -p 8080:80 nginx
   ```
This command starts a new container named mynginx in detached mode (-d) and maps port 8080 on the host to port 80 in the container (-p 8080:80).

3. Open a web browser and navigate to http://localhost:8080 to see the NGINX default page.

4. Stop and remove the container:
   ```bash
   $ podman stop mynginx

   $ podman rm mynginx
   ```
This stops and removes the mynginx container.
