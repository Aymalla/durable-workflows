# Container Orchestration

Containers are an excellent choice when developing software based on microservice architectures. They make efficient use of hardware, provide security features to run multiple instances simultaneously on the same host without affecting each other, and enable a service to be scaled out by deploying more instances.

![containers features](https://learn.microsoft.com/en-us/training/modules/intro-to-kubernetes/media/1-container-benefits.svg)

Advantages:

- **Potable:** Run on any Linux, Windows, or macOS machine
- **Efficiency:** Use less CPUs and memory, Saving Money
- **Isolation:** self-contained, can be spun up or down in seconds
- **Scalability:** Quick replications and elastically scale up and down

## Containers

A technology which pioneered and popularized by Docker

**Containers:** Bundles the application code, runtime and configuration required to run the code itself, in on unit.

**Container Image:** Container image is a file with executable code that can create a container on a computing system. A container image is immutable—meaning it cannot be changed, and can be deployed consistently in any environment. It is a core component of a containerized architecture. *Most modern container engines use the Open Container Initiative (OCI) container image format*

**Container Registry:** a repository used to store and access container images; these images can be available to the public or private.

**Container Engine:** a piece of software that accepts user requests, including command line options, pulls images, and from the end user's perspective runs the container. There are many container engines, including docker, RKT, CRI-O, and LXD. Container engines can run multiple, isolated instances, known as containers, on the same operating system kernel. Containers perform virtualization at the operating system level, and provide a controllable, easily manageable environment for running applications and dependencies.

## Kubernetes

Kubernetes (K8s) is an open source container orchestration platform written in Go, it's designed to provide planet-scale deployment, first release lunched by Google and Linux foundation on 2014.

- Kubernetes oversees a set of servers and decides where to deploy containerized applications, when to scale up and down the number of application replicas, and what to do when an application or server stops working.
- Kubernetes can run on any kind of server: on premise data center, public cloud or hybrid.
- Kubernetes used as stand-alone installation or Managed service by cloud provider.
- Kubernetes was the first graduated project by CNCF(Cloud native computing foundation)
