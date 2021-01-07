---
title: Go HandBooks
permalink: /handbooks/go/chapters/chap03/
---

## Build a Docker Image

This chapter explains how to create a Docker image.

### Dockerfile

Docker builds images by reading instructions from a _Dockerfile_.
A _Dockerfile_ is a text document that contains all the commands a user could call on the command line to assemble an image.

`docker image build` command uses this file and executes all the commands in succession to create an image.

`build` command is also passed a context that is used during image creation.
This context can be a path on your local filesystem or a URL to a Git repository.

_Dockerfile_ is usually called _Dockerfile_.
The complete list of commands that can be specified in this file are explained at [Dockerfile reference](https://docs.docker.com/engine/reference/builder/).
The common commands are listed below:

Common commands for Dockerfile
| Command | Purpose                                                                                                 | Example                            |
|---------|---------------------------------------------------------------------------------------------------------|------------------------------------|
| FROM    | First non-comment instruction in  _Dockerfile_                                                          | `FROM ubuntu`                      |
| COPY    | Copies mulitple source files from the context to the file system of the container at the specified path | `COPY .bash_profile /home`         |
| ENV     | Sets the environment variable                                                                           | `ENV HOSTNAME=test`                |
| RUN     | Executes a command                                                                                      | `RUN apt-get update`               |
| CMD     | Defaults for an executing container                                                                     | `CMD ["/bin/echo", "hello world"]` |
| EXPOSE  | Informs the network ports that the container will listen on                                             | `EXPOSE 8093`                      |
