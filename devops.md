# Devops

## 🔰 Introduction to DevOps
- DevOps is a combination of Development and Operations.
- It is a culture and set of practices that helps development teams and IT operations teams work together to deliver software faster, more reliably, and continuously.
- DevOps focuses on:
```
Automation
Collaboration
Continuous Integration & Continuous Delivery (CI/CD)
Faster feedback
High-quality software
```
- Goal: Reduce development time and increase deployment frequency with reliability.

<hr>

## 🌐 DevOps Ecosystem
- The DevOps ecosystem consists of tools and technologies used across the software lifecycle:

| Area                     | Popular Tools                      |
| ------------------------ | ---------------------------------- |
| Version Control          | Git, GitHub, GitLab, Bitbucket     |
| CI/CD                    | Jenkins, GitHub Actions, GitLab CI |
| Build Tools              | Maven, Gradle, npm                 |
| Containerization         | Docker                             |
| Orchestration            | Kubernetes                         |
| Configuration Management | Ansible, Chef, Puppet              |
| Cloud Platforms          | AWS, Azure, GCP                    |
| Monitoring & Logging     | Prometheus, Grafana, ELK Stack     |
| Infrastructure as Code   | Terraform, CloudFormation          |

- These tools work together to automate the entire pipeline from code to production.

<hr>

🔄 DevOps Phases (Lifecycle)
- DevOps follows a continuous cycle:
```
1.Plan
    Requirement analysis
    Project planning
    Tools: Jira, Trello
2.Develop
    Coding by developers
    Version control using Git
3.Build
    Compile and package code
    Tools: Maven, Gradle, Jenkins
4.Test
    Automated testing
    Tools: Selenium, JUnit
5.Release
    Prepare application for deployment
6.Deploy
    Deploy to servers or cloud
    Tools: Docker, Kubernetes, Ansible
7.Operate
    Run and manage application in production
8.Monitor
    Track performance and errors
    Tools: Prometheus, Grafana

🔁 Feedback from Monitor goes back to Plan — making DevOps a continuous loop.
```
- DevOps = Speed + Quality + Automation + Collaboration

<hr>

## 🔁 CI and CD in DevOps (Continuous Integration and Continuous Delivery / Continuous Deployment)

<img width="585" height="296" alt="image" src="https://github.com/user-attachments/assets/33c99a53-3c4e-4b01-a9a0-caea44c3d311" />

```
Stages 
Develop --> Build --> Testing --> Release[Deploy]

Testing
1. unit testing(do normally developers)
2. Integration testing
3. Regression testing (check new changes are work properly)

Release
1. dev
2. staging
3. production
```

Their two stages in CI and CD
- Build + Testing = CI
- Release[Deploy] = CD

- Integration hell = due to manual testing
- CI = It test and build in every commit of done by developer

- CD = their is remove of manual deployment

<hr>

## Docker

### 📦 Introduction to Containerisation
- Containerisation is a lightweight virtualization technique where an application <br>
and all its dependencies (libraries, frameworks, config files) are packed into a single unit called a container.

 ```
A container:
Runs the same on any system
Starts quickly
Uses fewer resources than Virtual Machines
Is isolated from other applications

Benefits:
“Works on my machine” problem solved
Fast deployment
Easy scaling
Better resource utilization
````

- Containers are portable , lightweight

### 🐳 Introduction to Docker
- Docker is the most popular containerisation platform.
- It allows you to build, ship, and run applications inside containers.
```
Key Docker Components:
Docker Image – Blueprint of an application
Docker Container – Running instance of an image
Docker Engine – Runs containers
Docker Hub – Public repository for images
```
Basic Commands:
```
docker --version
docker pull nginx
docker run nginx
docker ps
docker stop <container_id>

nginx - filename
```

### YAML (YAML Ain’t Markup Language)
- It is a human-readable data format used for configuration files in DevOps tools like Docker, Kubernetes, Ansible, GitHub Actions, etc.
```
Key Features:
Simple and easy to read
Uses indentation instead of brackets {}
Supports key–value pairs, lists, and objects
File extension: .yml or .yaml
```
Example:
```
version: "3"
services:
  web:
    image: nginx
    ports:
      - "80:80"
  app:
    image: node:18
    command: node app.js
```
Rules:

Indentation is important
No tabs (use spaces)
':' separates key and value
'-' is used for list items

YAML is widely used in:

Docker Compose

Kubernetes manifests

CI/CD pipelines

Cloud configurations

<hr>

## Docker Swarm
- Docker Swarm lets you run and manage containers on many servers together, like one big Docker host.

| Term             | Meaning                                   |
| ---------------- | ----------------------------------------- |
| **Node**         | A machine (VM or physical) running Docker |
| **Manager Node** | Controls the swarm, schedules tasks       |
| **Worker Node**  | Runs containers assigned by manager       |
| **Service**      | Definition of how containers should run   |
| **Task**         | A running container inside a service      |
| **Stack**        | Group of services (using YAML file)       |

```
🔹 Features of Docker Swarm
High availability
Load balancing (built-in)
Auto-scaling services
Rolling updates
Secure communication (TLS by default)
Easy setup compared to Kubernetes
```
Docker Swarm is commonly used in DevOps for container orchestration, microservices deployment, and high availability systems.

## Docket Stack
- Docker Stack is used in Docker Swarm to deploy and manage a group of services together using a YAML file (similar to docker-compose.yml).
- Docker Stack lets you deploy a complete multi-container application on a Swarm cluster with one command.

🔹 Difference: Docker Compose vs Docker Stack
| Docker Compose      | Docker Stack          |
| ------------------- | --------------------- |
| Single machine      | Multi-node cluster    |
| Dev/Testing         | Production            |
| `docker-compose up` | `docker stack deploy` |
| No orchestration    | Full orchestration    |

- Docker Stack is the production-level way to run multi-service applications in Docker Swarm.

<hr>

## Kubernetes
- Kubernetes (K8s) is an open-source container orchestration platform used to deploy, manage, and scale containerized applications across a cluster of machines.
- Kubernetes manages containers on many servers automatically – it deploys them, scales them, restarts them if they fail, and balances traffic.
- It is more powerful and flexible than Docker Swarm and is widely used in production.

🔹 Main Components
| Component                  | Purpose                                |
| -------------------------- | -------------------------------------- |
| **Cluster**                | Group of machines (nodes)              |
| **Master / Control Plane** | Manages the cluster                    |
| **Node (Worker)**          | Runs containers                        |
| **Pod**                    | Smallest unit (one or more containers) |
| **Deployment**             | Manages replicas & updates             |
| **Service**                | Exposes Pods (networking)              |
| **ConfigMap / Secret**     | App configuration                      |
| **Ingress**                | External access (HTTP/HTTPS)           |

🔹 Docker Swarm vs Kubernetes
| Docker Swarm      | Kubernetes             |
| ----------------- | ---------------------- |
| Easy to learn     | Complex but powerful   |
| Basic features    | Enterprise-grade       |
| Limited ecosystem | Huge ecosystem         |
| Small setups      | Large-scale production |

- Kubelet is an agent that runs on every worker node in a Kubernetes cluster.
- In simple words: Kubelet is responsible for making sure that the containers inside Pods are running properly on a node.

- Kube-Proxy is a network component that runs on every node in a Kubernetes cluster.
- In simple words: Kube-Proxy manages network rules so that Pods and Services can communicate with each other inside and outside the cluster.

```
User
  |
  |  (kubectl apply -f app.yaml)
  v
API Server  ←── All requests go here
  |
  v
etcd (stores cluster data)
  |
  v
Scheduler ── decides on which Node the Pod will run
  |
  v
Controller Manager ── ensures desired state (replicas, health)
  |
  v
Worker Node
   ├─ Kubelet ── creates & manages Pods
   ├─ Container Runtime ── runs containers
   └─ Kube-Proxy ── handles networking
```
