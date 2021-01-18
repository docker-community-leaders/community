---
title: Java HandBooks
permalink: /handbooks/java/chapters/chap01/
---


## Setup Environments

This section describes the hardware and software needed for this workshop, and how to configure them.
This workshop is designed for a BYOL (Bring Your Own Laptop) style hands-on-lab.

### Hardware & Software

- Memory: At least 4 GB+, strongly preferred 8 GB
- Operating System: Mac OS X (10.15.7+), Windows 10 Pro+ 64-bit, Ubuntu 20.04+, CentOS 7/8+.

_NOTE_: An older version of the operating system may be used.
The installation instructions would differ slightly in that case and are explained in the next section.



### Install Docker

Docker runs natively on Mac, Windows and Linux.

- If you're using Mac, go to this [link](https://www.docker.com/products/docker-desktop) and choose "Download for Mac" option
- If you're using Windows, go to this [link](https://www.docker.com/products/docker-desktop) and choose "Download for Windows" option
- If you're using Linux, select "View Linux Engine" to go this [link](https://hub.docker.com/search?q=&type=edition&offering=community&operating_system=linux) to download it for your preferred OS distro.

Most of the labs tutorials have been tested on Docker Desktop for Mac.

_NOTE_: Docker requires a fairly recent operating system version.



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
- Download and install Java IDE of your choice:
   - [NetBeans 8.2 `Java SE` version](https://netbeans.org/downloads/)
   - [IntelliJ IDEA Community or Ultimate](https://www.jetbrains.com/idea/download/)
   - [Eclipse IDE for Java EE Developers](https://www.eclipse.org/downloads/eclipse-packages/)
- Download and install [Maven] (https://maven.apache.org/download.cgi)
- Download the OpenJDK build of [JDK 9 for Linux x64](https://download.java.net/java/GA/jdk9/9/binaries/openjdk-9_linux-x64_bin.tar.gz)
- Download the early-access Open JDK build of [JDK 9 for Alpine Linux](https://jdk.java.net/9/)
