# ECS, ECR & Fargate - Docker in AWS

## Contents

-   [1. What is Docker?](#1-what-is-docker)
    -   [1.1 Where are Docker images stored?](#11-where-are-docker-images-stored)
    -   [1.2 Docker vs. Virtual Machines](#12-docker-vs-virtual-machines)
    

# 1. What is Docker?

-   Docker is a software development platform to **deploy apps**
-   Apps are packaged in containers that can be run on **any** OS
-   Apps run the same, regardless of where they’re run
    -   Any machine
    -   No compatibility issues
    -   Predictable behavior
    -   Less work
    -   Easier to maintain and deploy
    -   Works with any language, any OS, any technology
-   Use cases: microservices architecture, lift-and-shift apps from on- premises to the AWS cloud, …

<img src="images/dockerOnAnOS.PNG" style="height: 350px; width:450px;"/>

## 1.1 Where are Docker images stored?

-   Docker images are stored in **Docker Repositories**
-   Docker Hub (https://hub.docker.com)
    -   Public repository
    -   Find base images for many technologies or OS (e.g., Ubuntu, MySQL, …)
-   Amazon ECR (Amazon Elastic Container Registry)
    -   Private repository
    -   Public repository (Amazon ECR Public Gallery https://gallery.ecr.aws)

## 1.2 Docker vs. Virtual Machines

- Docker is ”sort of” a virtualization technology, but not exactly
- Resources are shared with the host => many containers on one server

<img src="images/DockerVsVirtualMachines.PNG"/>
