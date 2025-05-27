> From **Linux Foundation training**:
> https://training.linuxfoundation.org/training/introduction-to-kubernetes/

## Architecture principles

Microservices-based architecture is aligned with Event-driven Architecture and
Service-Oriented Architecture (SOA) principles, where complex applications are
composed of small independent processes which communicate with each other
through Application Programming Interfaces (APIs) over a network. APIs allow
access by other internal services of the same application or external,
third-party services and applications.

## Migration from monolithic to microservices

A so-called "Big-bang" approach focuses all efforts with the refactoring of the
monolith, postponing the development and implementation of any new features -
essentially delaying progress and possibly, in the process, even breaking the
core of the business, the monolith.

An incremental refactoring approach guarantees that new features are developed
and implemented as modern microservices which are able to communicate with the
monolith through APIs, without appending to the monolith's code. In the
meantime, features are refactored out of the monolith which slowly fades away
while all, or most its functionality is modernized into microservices. This
incremental approach offers a gradual transition from a legacy monolith to
modern microservices architecture and allows for phased migration of application
features into the cloud.

The refactoring phase slowly transforms the monolith into a cloud-native
application which takes full advantage of cloud features, by coding in new
programming languages and applying modern architectural patterns. Through
refactoring, a legacy monolith application receives a second chance at life - to
live on as a modular system adapted to fully integrate with today's fast-paced
cloud automation tools and services.

> Kubernetes User Case Studies: https://kubernetes.io/case-studies/

## Orchestration

- The controller/management unit is generally referred to as a **container
  orchestrator**.
- Containers encapsulate microservices and their dependencies but do not run
  them directly. Containers run container images.
- A container image bundles the application along with its runtime, libraries,
  and dependencies, and it represents the source of a container deployed to
  offer an isolated executable environment for the application. Containers can
  be deployed from a specific image on many platforms, such as workstations,
  Virtual Machines, public cloud, etc.
- From Dev environment to QA and Prod: Sometimes you might need to run
  containers on different hosts.
- Container orchestrators are tools which group systems together to form
  clusters where containers' deployment and management is automated at scale
  while meeting the requirements mentioned above.
- Some orchestration tools:
  - AWS Elastic Container Service (ECS)
  - Azure Container Instances (ACI)
  - Kubernetes, part of the Cloud Native Computing Foundation (CNCF) project
  - Docker Swarm, part of Docker Engine
- Container orchestrators are also explored in another Linux Foundation course,
  ["Introduction to Cloud Infrastructure Technologies (LFS151)"](https://training.linuxfoundation.org/training/introduction-to-cloud-infrastructure-technologies/).

## Deploy Container Orchestrators

- In addition, there are turnkey cloud solutions which allow production
  Kubernetes clusters to be installed, with only a few commands, on top of cloud
  Infrastructures-as-a-Service. These solutions paved the way for the managed
  container orchestration as-a-Service, more specifically the managed Kubernetes
  as-a-Service (KaaS) solution, offered and hosted by the major cloud providers.
  Examples of KaaS solutions are Amazon Elastic Kubernetes Service (Amazon EKS),
  Azure Kubernetes Service (AKS), DigitalOcean Kubernetes, Google Kubernetes
  Engine (GKE), IBM Cloud Kubernetes Service, Oracle Container Engine for
  Kubernetes, or VMware Tanzu Kubernetes Grid.
