---
title: Java HandBooks
permalink: /handbooks/java/chapters/chap01/
---


## Setup Environments

This section describes the hardware and software needed for this workshop, and how to configure them.
This workshop is designed for a BYOL (Bring Your Own Laptop) style hands-on-lab.

### Hardware & Software

- Memory: At least 4 GB+, strongly preferred 8 GB
- Operating System: Mac OS X (10.10.3+), Windows 10 Pro+ 64-bit, Ubuntu 12+, CentOS 7+.

_NOTE_: An older version of the operating system may be used.
The installation instructions would differ slightly in that case and are explained in the next section.

Amazon Web Services credentials with the [following permissions](https://docs.docker.com/docker-for-aws/iam-permissions/).
This is only needed for some parts of the workshop.

### Install Docker

Docker runs natively on Mac, Windows and Linux.
This lab will use [Docker Community Edition (CE)](https://www.docker.com/community-edition).
Download the Docker CE edition for your machine from the [Docker Store](https://store.docker.com/search?type=edition&offering=community).

_NOTE_: Docker CE requires a fairly recent operating system version.
If your machine does not meet the requirements, then you need to install [Docker Toolbox](https://www.docker.com/products/docker-toolbox).

This workshop is tested with Docker Community Edition `17.09.0-ce-rc2, build 363a3e7` on Mac OS X `10.12.5`.

### Download Images

This tutorial uses a few Docker images and software.
Let's download them before we start the tutorial.

Download the file from [docker-compose-pull-images.yml](https://raw.githubusercontent.com/docker/labs/master/developer-tools/java/scripts/docker-compose-pull-images.yml) and use the following command to pull the required images:

```
curl -O https://raw.githubusercontent.com/docker/labs/master/developer-tools/java/scripts/docker-compose-pull-images.yml
docker-compose -f docker-compose-pull-images.yml pull --parallel
```

_NOTE_: For Linux, `docker-compose` and `docker` commands need `sudo` access.
So prefix all commands with `sudo`.

### Other Software

The software in this section is specific to certain parts of the workshop.
Install them only if you plan to attempt them.

- Install [git](https://git-scm.com/)
- Install Docker Cloud CLI following the [instructions](https://docs.docker.com/docker-cloud/installing-cli/)
- Download and install Java IDE of your choice:
   - [NetBeans 8.2 `Java SE` version](https://netbeans.org/downloads/)
   - [IntelliJ IDEA Community or Ultimate](https://www.jetbrains.com/idea/download/)
   - [Eclipse IDE for Java EE Developers](https://www.eclipse.org/downloads/eclipse-packages/)
- Download and install [Maven] (https://maven.apache.org/download.cgi)
- Download the OpenJDK build of [JDK 9 for Linux x64](https://download.java.net/java/GA/jdk9/9/binaries/openjdk-9_linux-x64_bin.tar.gz)
- Download the early-access Open JDK build of [JDK 9 for Alpine Linux](https://jdk.java.net/9/)
