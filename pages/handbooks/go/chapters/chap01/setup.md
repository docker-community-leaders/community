---
title: Go HandBooks
permalink: /handbooks/go/chapters/chap01/
---


## Setup Environment

This section describes the hardware and software needed for this workshop, and how to configure them.
This workshop is designed for a BYOL (Bring Your Own Laptop) style hands-on-lab.

### Hardware & Software

- Memory: At least 4 GB+, strongly preferred 8 GB
- Operating System: Mac OS X (10.10.3+), Windows 10 Pro+ 64-bit, Ubuntu 12+, CentOS 7+.

### Install Docker

Docker runs natively on Mac, Windows and Linux.
This lab will use [Docker Community Edition (CE)](https://www.docker.com/community-edition).
Download the Docker CE edition for your machine from the [Docker Store](https://store.docker.com/search?type=edition&offering=community).

_NOTE_: Docker CE requires a fairly recent operating system version.
If your machine does not meet the requirements, then you need to install [Docker Toolbox](https://www.docker.com/products/docker-toolbox).

This workshop is tested with Docker Community Edition `19.03.13-ce-rc10, build fec3683` on Ubuntu `20.04.1 LTS`.

### Docker Images

This tutorial uses a few Docker images and software.
Let's download them before we start the tutorial.

In order to download the Docker images we will be using `docker-compose`.
You can install `docker-compose` following the instructions provided in the doc [here](https://docs.docker.com/compose/install/).

Now, download the [docker-compose-pull-images.yml](https://raw.githubusercontent.com/docker-community-leaders/alphasite/master/pages/handbooks/go/scripts/docker-compose-pull-images.yml) file and use the following command to pull the required images:

```
curl -O https://raw.githubusercontent.com/docker-community-leaders/alphasite/master/pages/handbooks/go/scripts/docker-compose-pull-images.yml
docker-compose -f docker-compose-pull-images.yml pull --parallel
```

### Other Software

The softwares in this section are specific to certain parts of the workshop.
Install them only if you plan to attempt them.

- Install [git](https://git-scm.com)
- Install [Go](https://golang.org/doc/install)
- Download and install a code editor of your choice:
   - [Visual Studio Code](https://code.visualstudio.com/download)
   - [GoLand](https://www.jetbrains.com/go/download/)
   - [Sublime Text](https://www.sublimetext.com/3)
