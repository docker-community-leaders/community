---
title: Docker101 HandBooks
permalink: /handbooks/docker101/
---

## What is this handbook for?

This is a community leader handbook to run Docker 101 workshop. This will cover every aspect of conducting workshop starting from setting up an event page till the completion of the successful workshop. 

### Features of this workshop

- Audience : 5 to 100
- Technical Skills Required : Basic knowledge of Linux, Basic concepts of Docker
- Length : 8 hours (including coffe and lunch breaks)


## Checklists 

### Before the workshop

S.No. | Name of Objectives | Status | 
:------------ | :-------------| :-------------|
1 | [Identify an Event Venue](/housekeeping/venue/README.md) |  ☑️ |
2 | [Planning an Event Agenda](/housekeeping/plan-an-event-agenda/README.md) |  ☑️ |
3 | [Setting up Event Registration Page](/housekeeping/event/README.md) | ☑️ |
4 | [Sending confirmation email for workshop](/housekeeping/email/README.md) |  ☑️ |


### During the workshop

S.No. | Name of Objectives | Status | 
:------------ | :-------------| :-------------|
5 | [Conducting Attendee Survey](/housekeeping/attendeesurvey/README.md) |  ☑️ |


### After the workshop

S.No. | Name of Objectives | Status | 
:------------ | :-------------| :-------------|
6 | [Post-Event FollowUp](/housekeeping/postevent/README.md) |  ☑️ |
7 | [Community Leader Survey](/housekeeping/clsurvey/README.md)  |  ☑️ |



## Recommended Agenda


| Description | Timing |
| --- | --- |
| Welcome | 8:45 AM to 9:00 AM |
| [Creating a DockerHub Account](dockerhub/dockerhub.md) | 9:00 AM to 9:15 AM |
| [Getting Started with Docker Image](#getting-started-with-docker-image---1-hour) | 9:15 AM to 10:15 AM |
| [Accessing & Managing Docker Container](#accessing-&-managing-docker-container---1-hour) | 10:15 AM to 11:15 AM |
| Coffee/Tea Break | 11:15 AM to 11:30 AM |
| [Getting Started with Dockerfile - Part 1](#getting-started-with-dockerfile---3-hours) | 11:30 AM to 1:00 PM|
| Lunch | 1:00 PM to 2:00 PM |
| Getting Started with Dockerfile| 2:00 PM to 3:30 PM |
| [Creating Private Docker Registry](#creating-private-docker-registry---30-min) | 3:30 PM to 4:00 PM|
| [Docker Volumes](#docker-volumes---30-min) | 4:00 PM to 4:30 PM |
| Coffee/Tea Break | 4:00 PM to 4:30 PM |
| [Docker Networking](#docker-networking---1-hour) | 4:45 PM to 5:45 PM |
| Quiz/Prize/Certificate Distribution | 5:45 PM to 6:00 PM |



## Pre-requisite:

- [Creating Your DockerHub Account](dockerhub/dockerhub.md) - 15 min

### Getting Started with Docker Image - 1 hour


- [Running Hello World Example](/helloworld/README.md)  
- [Working with Docker Image](/beginners/workingwithdockerimage/workingwithdockerimage.md) 
- [Saving Images and Containers as Tar Files for Sharing](/beginners/saving-images-as-tar/README.md)
- [Building Your First Alpine Docker Image and Push it to DockerHub](/building/building-your-first-alpine-container.md)
- [Test Your Knowledge](/beginners/quiz1/README.md)



###  Accessing & Managing Docker Container - 1 hour

- [Accessing the Container Shell](/beginners/accessing-the-container/README.md)<br>
- [Running a Command inside running Container](/beginners/running-command-inside-running-container/README.md)<br>
- [Managing Docker Containers](/beginners/managing-containers/README.md)<br>
- [Test Your Knowledge](/beginners/quiz2/README.md)


### Getting Started with Dockerfile - 3 hours

- [What is Dockerfile](/beginners/dockerfile/Writing-dockerfile/README.md)<br>
- [Understanding Layering Concept with Dockerfile](/beginners/dockerfile/Layering-Dockerfile/README.md)
- Creating Docker Image with
   - [Lab #1: Installing GIT](/beginners/dockerfile/lab1_dockerfile_git/README.md)<br>
   - [Lab #2: ADD instruction](/beginners/dockerfile/Lab-2-Create-an-image-with-ADD-instruction/README.md)<br>
   - [Lab #3: COPY instruction](/beginners/dockerfile/lab4_dockerfile_copy/README.md)<br>
   - [Lab #4: CMD instruction](/beginners/dockerfile/lab4_cmd/README.md)<br>
   - [Lab #5: ENTRYPOINT instruction](/beginners/dockerfile/Dockerfile-ENTRYPOINT/README.md)<br>
   - [Lab #6: WORKDIR instruction](/beginners/dockerfile/WORKDIR_instruction/README.md)<br>
   - [Lab #7: RUN instruction](/beginners/dockerfile/Lab-7-Create-an-image-with-EXPOSE-instruction/README.md)<br>
   - [Lab #8: ARG instruction](/beginners/dockerfile/arg/README.md)<br>
   - [Lab #9: ENV instruction](/beginners/dockerfile/Lab_ENV_instruction/README.md)<br>
   - [Lab #10: VOLUME instruction](/beginners/dockerfile/Lab_VOLUME_instruction/README.md)<br>
   - [Lab #11: EXPOSE instruction](/beginners/dockerfile/Lab_EXPOSE_instruction/README.md)<br>
   - [Lab #12: LABEL instruction](/beginners/dockerfile/Label_instruction/README.md)<br>
   - [Lab #13: ONBUILD instruction](/beginners/dockerfile/onbuild/README.md)<br>
   - [Lab #14: HEALTHCHECK instruction](/beginners/dockerfile/healthcheck/README.md)<br>
   - [Lab #15: SHELL instruction](/beginners/dockerfile/Lab-14-Create-an-image-with-SHELL-instruction/README.md)<br>
   - [Lab #16: Entrypoint Vs RUN](/beginners/dockerfile/entrypoint-vs-run/README.md)<br>
   - [Lab #17: USER instruction](/beginners/dockerfile/user/README.md)
- [Writing Dockerfile with Hello Python Script Added](/beginners/dockerfile/lab_dockerfile_python/README.md)<br>
- [Test Your Knowledge](/beginners/dockerfile/quiz3/README.md)

### Creating Private Docker Registry - 30 min

- [Building a Private Docker Registry](/beginners/build-private-docker-registry/README.md)
- [Test Your Knowledge](/beginners/quiz3/README.md)

### Docker Volumes - 30 min

- [Managing volumes through Docker CLI](/beginners/volume/managing-volumes-via-docker-cli/README.md)<br>
- [Creating Volume Mount from **docker run** command & sharing same Volume Mounts among multiple containers](/beginners/volume/creating-volume-mount-from-dockercli/README.md)<br>
- [Test Your Knowledge](/beginners/volume/quiz4/README.md)

### Docker Networking - 1 hour

 - [The docker network Command](/beginners/networking/using-docker-network/README.md)<br>
 - [Lab #1: Listing the Networks](/beginners/networking/A1-network-basics.html#step-2-list-networks)
 - [Lab #2: Inspecting a Network](/beginners/networking/A1-network-basics.html#step-3-inspect-a-network)
 - [Lab #3: List network driver plugins](/beginners/networking/A1-network-basics.html#step-4-list-network-driver-plugins)
 - [Lab #4: Docker Bridge Networking](/beginners/networking/A2-bridge-networking.html)
   - [Lab #5: Basics of Docker Bridge Networking](/beginners/networking/A2-bridge-networking.html#step-1-the-default-bridge-network)
   - [Lab #6: Connect a Docker container to bridge network](/beginners/networking/A2-bridge-networking.html#step-2-connect-a-container)
   - [Lab #7: Test Network Connectivity](/beginners/networking/A2-bridge-networking.html#step-3-test-network-connectivity)
   - [Lab #8: Configure NAT for external connectivity](/beginners/networking/A2-bridge-networking.html#step-4-configure-nat-for-external-connectivity)
 - [Test Your Knowledge](/beginners/networking/quiz5/README.md)


