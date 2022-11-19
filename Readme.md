## What is docker?

```
A platform for building, running and shipping applications.
Consistently build, run and ship applications
```

It works on my machine.

# Reasons

1. One or more files are missing. Not completely deployed.
2. Software version mismatch.
3. Different configuration settings.

With docker you can easily package your application with everything that you need and run it anywhere on any machine with docker.

## Virtual Machines Vs Containers.

Container: is an isolated environment for running an application.

1. Allow running multiple apps in isolation.
2. Are lightweight.
3. Use OS of the host.
4. Start quickly.
5. Need less hardware resources.

Virtual Machines: An abstraction of a machine. aka Physical hardware.

## Docker Architecture

1. Uses Client Server Architecture. So it has a client component that talks to the server component using a RESTFUL API

## Install Docker

1. https://docs.docker.com

## Development Workflow

1. Dockerize the application by adding a Dockerfile which is a plain text file. Docker uses this file to package the application to an image. The image containes everything that needs to run the application.
2. Image contains: A cut-down OS, A runtime environment, application files, Third party libraries, Environment variables.

## Instructions to run Docker

1. Start with an OS
2. Install node.
3. copy app files.
4. Run node app.js

## Official docker image link : https://hub.docker.com/search?q=node

1. Linux distribution (eg. alpine)
   ```
   FROM node:alpine
   COPY ./app
   WORKDIR /app
   CMD node app.js
   ```
