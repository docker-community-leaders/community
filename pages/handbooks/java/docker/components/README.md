---
title: Java HandBooks
permalink: /handbooks/java/docker/components/
---


##  Docker Basic Concepts

This section introduces the basic terminology of Docker.


Docker is a platform for developers and sysadmins to build, ship, and run applications. Docker lets you quickly assemble applications from components and eliminates the friction that can come when shipping code. Docker lets you test and deploy your code into production as fast as possible.

Docker simplifies software delivery by making it easy to build and share images that contain your application’s entire environment, or _application operating system_.

## What does it mean by an application operating system ?

Your application typically requires specific versions for your operating system, application server, JDK, and database server, may require to tune the configuration files, and similarly multiple other dependencies. The application may need binding to specific ports and certain amount of memory. The components and configuration together required to run your application is what is referred to as application operating system.

You can certainly provide an installation script that will download and install these components. Docker simplifies this process by allowing to create an image that contains your application and infrastructure together, managed as one component. These images are then used to create Docker containers which run on the container virtualization platform, provided by Docker.

## Main Components

Docker has three main components:

- Images are the *build component* of Docker and are the read-only templates defining an application operating system.
- Containers are the *run component* of Docker and created from images. Containers can be run, started, stopped, moved, and deleted.
- Images are stored, shared, and managed in a registry and are the *distribution component* of Docker. 
- DockerHub is a publicly available registry and is available at http://hub.docker.com.

In order for these three components to work together, the *Docker Daemon* (or Docker Engine) runs on a host machine and does the heavy lifting of building, running, and distributing Docker containers. In addition, the *Client* is a Docker binary which accepts commands from the user and communicates back and forth with the Engine.

.Docker architecture
image::docker-architecture.png[]

The Client communicates with the Engine that is either co-located on the same host or on a different host. Client uses the `pull` command to request the Engine to pull an image from the registry. The Engine then downloads the image from Docker Store, or whichever registry is configured. Multiple images can be downloaded from the registry and installed on the Engine. Client uses the `run` run the container.

