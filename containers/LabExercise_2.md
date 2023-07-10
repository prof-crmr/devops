# Exercise 2: Creating a Custom Image and Running
## Objective: Learn how to create a custom Docker image and run a container from it using Podman.

1. Create a new directory for your custom image and navigate into it:

$ mkdir myimage
$ cd myimage

2. Create a Dockerfile using a text editor:

FROM alpine:latest
RUN apk update && apk add --no-cache nginx
COPY index.html /usr/share/nginx/html/
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]

This Dockerfile starts from the latest Alpine Linux image, installs NGINX, copies a custom index.html file, exposes port 80, and sets the command to start NGINX.

3. Create the index.html file using a text editor:

<html>
<body>
<h1>Hello, Container World!</h1>
</body>
</html>

This file will be copied into the container to replace the default NGINX page.

4. Build the Docker image:

$ podman build -t myimage .

This command builds the Docker image using the current directory (.) and tags it with the name myimage.

5. Run a container from your custom image:

$ podman run --name mycontainer -d -p 8080:80 myimage

This starts a new container named mycontainer using the myimage image and maps port 8080 on the host to port 80 in the container.

6. Open a web browser and navigate to http://localhost:8080 to see your custom web page.

7. Stop and remove the container:

$ podman stop mycontainer

$ podman rm mycontainer

This stops and removes the mycontainer container.

Congratulations! You have completed the Container Training Labs. You've accomplished the objectives of running an image using NGINX and creating a custom image using Podman. Feel free to explore more features and experiment with different containers and images using Podman.

Note: If you're using a different port in the exercises, make sure to adjust the instructions accordingly.
