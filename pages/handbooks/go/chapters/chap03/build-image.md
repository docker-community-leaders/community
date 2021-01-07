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

| Command | Purpose                                                                                                 | Example                            |
|---------|---------------------------------------------------------------------------------------------------------|------------------------------------|
| FROM    | First non-comment instruction in  _Dockerfile_                                                          | `FROM ubuntu`                      |
| COPY    | Copies mulitple source files from the context to the file system of the container at the specified path | `COPY .bash_profile /home`         |
| ENV     | Sets the environment variable                                                                           | `ENV HOSTNAME=test`                |
| RUN     | Executes a command                                                                                      | `RUN apt-get update`               |
| CMD     | Defaults for an executing container                                                                     | `CMD ["/bin/echo", "hello world"]` |
| EXPOSE  | Informs the network ports that the container will listen on                                             | `EXPOSE 8093`                      |

### Create your first image

Create a new directory `helloworld`.

In that directory, create a new text file `Dockerfile`. Use the following contents:

```
FROM ubuntu:latest

CMD ["/bin/echo", "hello world"]
```

This image uses `ubuntu` as the base image.
`CMD` command defines the command that needs to run.
It provides a different entry point of `/bin/echo` and gives the argument "`hello world`".

Build the image using the command:

```
docker image build -t helloworld .
```

`.` in this command is the context for the command `docker image build`. `-t` adds a tag to the image.

The following output is shown:

```
Sending build context to Docker daemon  2.048kB
Step 1/2 : FROM ubuntu:latest
latest: Pulling from library/ubuntu
9fb6c798fa41: Pull complete 
3b61febd4aef: Pull complete 
9d99b9777eb0: Pull complete 
d010c8cf75d7: Pull complete 
7fac07fb303e: Pull complete 
Digest: sha256:31371c117d65387be2640b8254464102c36c4e23d2abe1f6f4667e47716483f1
Status: Downloaded newer image for ubuntu:latest
 ---> 2d696327ab2e
Step 2/2 : CMD /bin/echo hello world
 ---> Running in 9356a508590c
 ---> e61f88f3a0f7
Removing intermediate container 9356a508590c
Successfully built e61f88f3a0f7
Successfully tagged helloworld:latest
```

List the images available using `docker image ls`:

```
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
helloworld          latest              14f96be609c4        3 minutes ago       72.9MB
ubuntu              latest              9140108b62dc        3 days ago          72.9MB
```

Other images may be shown as well but we are interested in these two images for now.

Run the container using the command:

```
docker container run helloworld
```

to see the output:

```
hello world
```

If you do not see the expected output, check your Dockerfile that the content exactly matches as shown above.
Build the image again and now run it.

Change the base image from `ubuntu` to `busybox` in `Dockerfile`. Build the image again:

```
docker image build -t helloworld:2 .
```

and view the images using `docker image ls` command:

```
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
helloworld          2                   9b9337b0efb1        15 seconds ago       1.24MB
helloworld          latest              14f96be609c4        3 minutes ago       72.9MB
ubuntu              latest              9140108b62dc        3 days ago          72.9MB
busybox             latest              a77dce18d0ec        8 days ago          1.24MB
```

`helloworld:2` is the format that allows to specify the image name and assign a tag/version to it separated by `:`.

Run the container using the command:

```
docker container run helloworld:2
```

Congratulations! You have successfully built and run your first Docker container.
