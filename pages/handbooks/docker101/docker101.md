---
title: Docker101 HandBooks
permalink: /handbooks/docker101/
---

## What is this handbook all about?

This is a community leader handbook to run Docker 101 workshop. This will cover every aspect of conducting workshop starting from setting up an event page till the completion of the successful workshop. 

### Key Characteristics of this workshop

- Audience - 5 to 100
- Technical Skills Required - Basic knowledge of Linux, Basic concepts of Docker
- Length - 8 hours


## Where/When/Who?

- [Identify an event venue](/housekeeping/identify-an-event-venue/README.md)
- [Plan an event agenda](/housekeeping/plan-an-event-agenda/README.md)
- [Set up Event Registration Page](/housekeeping/event/README.md)
- [Sending Confirmation Email for workshop](/housekeeping/email/README.md)
- [Prepare Checklists for Docker Workshop](/housekeeping/checklist/README.md)
- [Community Leader Survey](/housekeeping/clsurvey/README.md)
- [Attendee Survey](/housekeeping/attendeesurvey/README.md)


## Recommended Agenda

- Welcome (8:45 AM to 9:00 AM)
- Creating a DockerHub Account(9:00 AM to 9:15 AM)
- Getting Started with Docker Image(9:15 AM to 10:15 AM)
- Accessing & Managing Docker Container(10:15 AM to 11:15 AM)
- Coffee/Tea Break(11:15 AM to 11:30 AM)
- Getting Started with Dockerfile - Part 1(11:30 AM to 1:00 PM) 
- Lunch(1:00 PM to 2:00 PM)
- Getting Started with Dockerfile - Part 2(2:00 PM to 3:30 PM)
- Creating Private Docker Registry ( 3:30 PM to 4:00 PM)
- Docker Volumes(4:00 PM to 4:30 PM)
- Coffee/Tea Break(4:30 PM to 4:45 PM)
- Docker Networking(4:45 PM to 5:45 PM)
- Quiz/Prize/Certificate Distribution (5:45 PM to 6:00 PM)

## Pre-requisite:

- [Creating Your DockerHub Account](dockerhub/dockerhub.md) - 15 min

### Getting Started with Docker Image - 1 hour


- [Running Hello World Example](/helloworld/README.md)  
- [Working with Docker Image](/beginners/workingwithdockerimage/workingwithdockerimage.md) 
- [Saving Images and Containers as Tar Files for Sharing](/beginners/saving-images-as-tar/README.md)
- [Building Your First Alpine Docker Image and Push it to DockerHub](/building/building-your-first-alpine-container.md)

- Tips & Tricks()



###  Accessing & Managing Docker Container - 1 hour

- [Accessing the Container Shell](/beginners/accessing-the-container/README.md)<br>
- [Running a Command inside running Container](/beginners/running-command-inside-running-container/README.md)<br>
- [Managing Docker Containers](/beginners/managing-containers/README.md)<br>

- Tips & Tricks()


### Getting Started with Dockerfile - 3 hours

- [What is Dockerfile](/beginners/dockerfile/Writing-dockerfile.html#what-is-a-dockerfile)<br>
- [Understanding Layering Concept with Dockerfile](/beginners/dockerfile/Layering-Dockerfile.html)
- Creating Docker Image with
   - [Lab #1: Installing GIT](/beginners/dockerfile/lab1_dockerfile_git.html)<br>
   - [Lab #2: ADD instruction](/beginners/dockerfile/Lab-2-Create-an-image-with-ADD-instruction.html)<br>
   - [Lab #3: COPY instruction](/beginners/dockerfile/lab4_dockerfile_copy.html)<br>
   - [Lab #4: CMD instruction](/beginners/dockerfile/lab4_cmd.html)<br>
   - [Lab #5: ENTRYPOINT instruction](/beginners/dockerfile/Dockerfile-ENTRYPOINT.html)<br>
   - [Lab #6: WORKDIR instruction](/beginners/dockerfile/WORKDIR_instruction.html)<br>
   - [Lab #7: RUN instruction](/beginners/dockerfile/Lab-7-Create-an-image-with-EXPOSE-instruction.html)<br>
   - [Lab #8: ARG instruction](/beginners/dockerfile/arg.html)<br>
   - [Lab #9: ENV instruction](/beginners/dockerfile/Lab_%239:ENV_instruction.html)<br>
   - [Lab #10: VOLUME instruction](/beginners/dockerfile/Lab%2310:VOLUME_instruction.html)<br>
   - [Lab #11: EXPOSE instruction](/beginners/dockerfile/Lab%2311:EXPOSE_instruction.html)<br>
   - [Lab #12: LABEL instruction](https://dockerlabs.collabnix.com/beginners/dockerfile/Label_instruction.html)<br>
   - [Lab #13: ONBUILD instruction](https://dockerlabs.collabnix.com/beginners/dockerfile/onbuild.html)<br>
   - [Lab #14: HEALTHCHECK instruction](https://dockerlabs.collabnix.com/beginners/dockerfile/healthcheck.html)<br>
   - [Lab #15: SHELL instruction](https://dockerlabs.collabnix.com/beginners/dockerfile/Lab-14-Create-an-image-with-SHELL-instruction.html)<br>
   - [Lab #16: Entrypoint Vs RUN](https://dockerlabs.collabnix.com/beginners/dockerfile/entrypoint-vs-run.html)<br>
   - [Lab #17: USER instruction](https://dockerlabs.collabnix.com/beginners/dockerfile/user.html)
- [Writing Dockerfile with Hello Python Script Added](https://dockerlabs.collabnix.com/beginners/dockerfile/lab_dockerfile_python.html)<br>

- Tips & Tricks()

### Creating Private Docker Registry - 30 min

- [Building a Private Docker Registry](https://dockerlabs.collabnix.com/beginners/build-private-docker-registry.html)
- [Building a Private Docker Registry with UI](https://dockerlabs.collabnix.com/beginners/portus/)

- Tips & Tricks()

### Docker Volumes - 30 min

- [Managing volumes through Docker CLI](https://collabnix.github.io/dockerlabs/beginners/volume/managing-volumes-via-docker-cli.html)<br>
- [Creating Volume Mount from **docker run** command & sharing same Volume Mounts among multiple containers](https://collabnix.github.io/dockerlabs/beginners/volume/creating-volume-mount-from-dockercli.html)<br>

- Tips & Tricks()

### Docker Networking - 1 hour

 - [The docker network Command](http://dockerlabs.collabnix.com/beginners/using-docker-network.html)<br>
 - [Lab #1: Listing the Networks](http://dockerlabs.collabnix.com/networking/A1-network-basics.html#step-2-list-networks)
 - [Lab #2: Inspecting a Network](http://dockerlabs.collabnix.com/networking/A1-network-basics.html#step-3-inspect-a-network)
 - [Lab #3: List network driver plugins](http://dockerlabs.collabnix.com/networking/A1-network-basics.html#step-4-list-network-driver-plugins)
 - [Lab #4: Docker Bridge Networking](http://dockerlabs.collabnix.com/networking/A2-bridge-networking.html)
   - [Lab #5: Basics of Docker Bridge Networking](http://dockerlabs.collabnix.com/networking/A2-bridge-networking.html#step-1-the-default-bridge-network)
   - [Lab #6: Connect a Docker container to bridge network](http://dockerlabs.collabnix.com/networking/A2-bridge-networking.html#step-2-connect-a-container)
   - [Lab #7: Test Network Connectivity](http://dockerlabs.collabnix.com/networking/A2-bridge-networking.html#step-3-test-network-connectivity)
   - [Lab #8: Configure NAT for external connectivity](http://dockerlabs.collabnix.com/networking/A2-bridge-networking.html#step-4-configure-nat-for-external-connectivity)
 
 - Tips & Tricks() - Highlights/AttentionGrabber


