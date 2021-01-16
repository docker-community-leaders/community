---
title: Dockerizing your application for Java 
permalink: /handbooks/java/
---

## What is this handbook for?

This is a community leader handbook to run "Dockerizing Your Application for JAVA" workshop. This will cover every aspect of conducting workshop starting from setting up an event page till the completion of the successful workshop. 

### Features of this workshop

- Audience : 5 to 100
- Technical Skills Required : Basic knowledge of Linux & JAVA
- Length : 4 hours (including coffe and lunch breaks)


## Checklists 

### Before the workshop

S.No. | Name of Objectives | Status | 
:------------ | :-------------| :-------------|
1 | [Getting Familiar with Bevy Virtual](/housekeeping/virtual/README.md) |  ☑️ |
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
| [Setting up Infrastructure](java/infrastructure/README.md) | 9:00 AM to 9:30 AM |
| [Basics of Docker](#basics-of-docker---1-hour) | 9:30 AM to 10:30 AM |
| [Building a Docker Image](#building-a-docker-image---1-hour) | 10:15 AM to 11:15 AM |
| Coffee/Tea Break | 11:15 AM to 11:30 AM |
| [Building a Docker Image for Java 11](#building-a-docker-image-for-java-11---1-hour) | 11:30 AM to 12:30 PM|
| Lunch | 1:00 PM to 2:00 PM |
| [Multi-container Application using Docker Compose](#multi-container-application-using-docker-compose---30-min) | 3:30 PM to 4:30 PM|
| [Multi-container Application using Docker Compose & Swarm Mode](#multi-container-application-using-docker-compose-and-swarm---30-min) | 4:00 PM to 4:30 PM |
| Coffee/Tea Break | 4:00 PM to 4:30 PM |
| [Java IDE](#java-ide---1-hour) | 4:45 PM to 5:45 PM |
| [CI-CD using Docker](#ci-cd-using-docker) | 5:45 PM to 6:00 PM |



## Pre-requisite:

### [Setting up Infrastructure](#setting-up-infrastructure) - 30 min

- [Hardware & Software](/infra/hardware/README.md)
- [Installing Docker](/infra/installing-docker/README.md)
- [Downloading the required Docker Images](/infra/downloading-docker-images/README.md)
- [Installing Other Software](/infra/installing-other-software/README.md)
- [Test Your Knowledge](infra/quiz1/README.md)


### [Basics of Docker](#basics-of-docker) - 30 min
- [Main Components](/docker/components/README.md)
- [Docker Image](/docker/docker-image/README.md)
- [Docker Container](/docker/docker-container/README.md)
- [Docker Engine](/docker/docker-engine/README.md)
- [Docker Client](/docker/docker-client/README.md)
- [Test Your Knowledge](/docker/infra/quiz2/README.md)


### [Building and Running a Docker Container](#building-and-running-a-docker-container) - 1 hour
 - [Build a Docker Image](/docker/build-a-docker-image/README.md)
 - [Build a Docker Image for JAVA 11](/docker/build-a-docker-image/README.md)
 - [Running a JAVA 11 Docker Container](/docker/running-a-JAVA-11-docker-container/README.md)


### [Multi-Container Application using Docker Compose](#multi-container-application-using-docker-compose) - 1 hour
- [What is Docker Compose](/compose/what-is-docker-compose/README.md)
- [Configuration file](/compose/configuration/README.md)
- [Start application](/compose/start/README.md)
- [Verify application](/compose/verify/README.md)
- [Shutdown application](/compose/shutdown/README.md)


### Deploy Application using Docker Swarm Mode
- [Initialize Swarm](/swarm/initialize-swarm/README.md)
- [Multi-container application](/swarm/multicontainer/README.md)
- [Verify service and containers in application](/swarm/verify//README.md)
- [Access application](/swarm/access/README.md)
- [Stop application](/swarm/stop-/README.md)
- [Remove application completely](/swarm/remove/README.md)


### Docker & Netbeans
- [Configure Docker Host](/netbeans/configure/README.md)
- [Pull an Image](/netbeans/pull/README.md)
- [Run a Container](/netbeans/run/README.md)
- [Build an Image](/netbeans/build/README.md)


### Docker and IntelliJ IDEA
- [Install Docker Plugin in IDEA](/intellij/install-docker-plugin/README.md)
- [Pull an Image](/intellij/pull/README.md)
- [Run a Container](/intellij/run/README.md)
- [Build an Image](/intellij/build/README.md)






