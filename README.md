# DevOps & Cloud Engineering — Hands-on Project Portfolio

## Portfolio Overview

This portfolio documents my hands-on transition into **DevOps and Cloud Engineering**, combining cloud infrastructure, Infrastructure as Code, CI/CD, DevSecOps, containerization, Kubernetes, automation, networking, monitoring, and troubleshooting.

My approach is project-based and implementation-focused, with emphasis on **designing, deploying, securing, monitoring, verifying, and troubleshooting** applications and infrastructure across AWS and local development environments.

The portfolio complements my previous background in channel sales and business development by combining **technical problem-solving, cloud engineering, automation, security, and business awareness**.

---

## Technical Focus

* ☁️ **Cloud Engineering:** AWS, EC2, VPC, IAM, S3, RDS, ECR, EKS
* 🏗️ **Infrastructure as Code:** Terraform
* ⚙️ **Automation:** Ansible, Bash, Linux, Python
* 🔄 **CI/CD:** Jenkins, GitHub, automated testing
* 🔐 **DevSecOps:** SonarCloud, Snyk, Trivy, OWASP ZAP
* 🐳 **Containers:** Docker, Docker Compose
* ☸️ **Orchestration:** Kubernetes, Amazon EKS
* 📊 **Observability:** Prometheus, Grafana, application metrics and health checks
* 🔧 **Operations:** AWS CLI, kubectl, Git, Linux troubleshooting

---

# Featured Projects

## 1. End-to-End Node.js CI/CD & DevSecOps Pipeline on AWS

An end-to-end DevOps and DevSecOps implementation demonstrating the software delivery lifecycle from source code through testing, security validation, containerization, artifact publishing, Kubernetes deployment, and runtime security testing.

### Technologies

**GitHub • Jenkins • Node.js • Jest • SuperTest • SonarCloud • Snyk • Docker • Trivy • Amazon ECR • Amazon EKS • OWASP ZAP • Terraform • Prometheus • Grafana**

### Key Capabilities

* Automated CI/CD pipeline using Jenkins and GitHub
* Jest and SuperTest automated testing
* SonarCloud SAST and Quality Gate enforcement
* Snyk Software Composition Analysis
* Docker containerization
* Trivy container image vulnerability scanning
* Amazon ECR authentication, image publishing, and verification
* Kubernetes/EKS deployment and validation
* OWASP ZAP DAST against the running application
* Application health and Prometheus metrics endpoints
* Prometheus/Grafana monitoring
* AWS infrastructure provisioned with Terraform

**Detailed implementation:** See the project's `README.md` for architecture, configuration, pipeline stages, security results, deployment evidence, verification, and troubleshooting.

[View Project Repository](https://github.com/Jefferson-ohis1/end-to-end-node-ci-cd-devsecops.git)

> An end-to-end DevOps and DevSecOps implementation.

---

## 2. Java DevSecOps CI/CD Pipeline

A containerized Java application delivery pipeline implementing DevSecOps practices across the software development lifecycle.

### Technologies

**Java • Jenkins • Docker • SonarCloud • Snyk • Trivy • OWASP ZAP • AWS EC2**

### Key Capabilities

* Jenkins-based CI/CD automation
* Docker application containerization
* SonarCloud SAST
* Snyk dependency security analysis
* Trivy container vulnerability scanning
* OWASP ZAP DAST
* Automated application build and delivery
* Shift-Left Security practices

**Detailed implementation:** See the project's `README.md` for the complete pipeline, security controls, configuration, results, and implementation evidence.


[View Project Repository](https://github.com/Jefferson-ohis1/java-devsecops-ci-cd-pipeline.git)

> A containerized Java application delivery pipeline.

---

## 3. AWS Infrastructure with Terraform

Hands-on Infrastructure as Code experience focused on provisioning and managing AWS infrastructure through repeatable and version-controlled Terraform configurations.

### AWS Resources

* Amazon VPC
* Public and private subnets
* Route tables
* Internet Gateway
* Security groups
* IAM roles and permissions
* EC2
* Amazon ECR
* Amazon EKS
* Supporting networking and infrastructure resources

### Practical Experience

* Terraform-based infrastructure provisioning
* Resource dependency management
* Infrastructure verification
* Terraform state management
* AWS networking troubleshooting
* Resource lifecycle management
* Troubleshooting provisioning and destruction dependencies

[View Project Repository](https://github.com/Jefferson-ohis1/Infrastructure-as-code-Terraform.git)

---

## 4. Automated Nginx Website Deployment with Ansible

Ansible automation project demonstrating configuration management and repeatable website deployment across multiple AWS EC2 instances.

### Technologies

**Ansible • AWS EC2 • Linux • Nginx • SSH**

### Key Capabilities

* Ansible inventory and playbook configuration
* Automated Nginx installation
* Nginx service configuration
* Service start and enablement
* Static website deployment
* Multi-host deployment
* Deployment verification
* SSH-based remote automation

[View Project Repository](https://github.com/Jefferson-ohis1/Ansible-nginx-static-website-deployment.git)

---

## 5. Three-Tier Kanban Application with Docker Compose

A multi-container application demonstrating practical container orchestration and communication between application tiers.

### Architecture

```text
Angular Frontend
       │
       ▼
Java / Spring Boot Backend
       │
       ▼
PostgreSQL Database
```

### Technologies

**Angular • Java • Spring Boot • PostgreSQL • Docker • Docker Compose**

### Key Capabilities

* Multi-container application architecture
* Docker image creation
* Docker Compose orchestration
* Container networking
* Port mapping
* Service dependencies
* PostgreSQL persistent storage
* Application configuration
* Container lifecycle management
* Multi-tier application troubleshooting

[View Project Repository](https://github.com/Jefferson-ohis1/Using-Docker-compose-To-Deploy-A-Three-Tier-App-Kanban-App.git)

---

## 6. WordPress Two-Tier Application with Docker Compose

A Docker Compose project demonstrating deployment of a multi-container WordPress application.

### Key Capabilities

* WordPress containerization
* Database containerization
* Docker Compose orchestration
* Container networking
* Environment configuration
* Persistent storage
* Service dependencies
* Multi-container troubleshooting

[View Project Repository](https://github.com/Jefferson-ohis1/Using-Docker-compose-To-Deploy-A-Two-Tier-App-WordPress-App.git)

---

# AWS Cloud & Infrastructure Experience

My hands-on AWS work includes designing, provisioning, configuring, and troubleshooting cloud infrastructure.

### Compute

* Amazon EC2
* Linux server configuration
* SSH access
* HTTP application access
* Security groups
* Launch Templates
* Auto Scaling Groups

### Networking

* Amazon VPC
* Public and private subnets
* Route tables
* Internet Gateway
* Security groups
* Load Balancers
* Network traffic flow and connectivity troubleshooting

### Storage & Databases

* Amazon S3
* Object upload and management
* Static website hosting
* Cross-region replication
* Amazon RDS MySQL

### Identity & Security

* AWS IAM users and groups
* Permissions and access controls
* IAM roles
* EC2 access controls
* Security groups
* SSH access

### Containers & Kubernetes

* Amazon ECR
* Amazon EKS
* Container image publishing
* ECR image verification
* Kubernetes workload deployment

### Cost Management

* AWS Cost Explorer
* AWS Budgets
* Basic cloud cost monitoring and budgeting

### AWS Operations

* AWS CLI
* Resource inspection
* Configuration
* Authentication
* Verification
* Troubleshooting

---

# Infrastructure as Code & Automation

## Terraform

Used Terraform to provision and manage AWS infrastructure using repeatable, version-controlled Infrastructure as Code practices.

Experience includes:

* AWS networking
* IAM
* EC2
* Amazon ECR
* Amazon EKS
* Supporting AWS resources
* Resource dependencies
* Infrastructure verification
* Terraform lifecycle management
* Troubleshooting provisioning and destruction issues

## Ansible

Used Ansible for configuration management and automated deployment across AWS EC2 instances.

Experience includes:

* Inventory management
* Playbook development
* Nginx installation
* Service configuration
* Website deployment
* Multi-host automation
* Deployment verification

---

# CI/CD & DevSecOps

Hands-on CI/CD experience includes both **Node.js and Java application pipelines** using Jenkins and GitHub.

### CI/CD Workflow

```text
GitHub
   ↓
Jenkins
   ↓
Automated Testing
   ↓
SonarCloud SAST
   ↓
Snyk SCA
   ↓
Docker Build
   ↓
Trivy Container Scan
   ↓
Amazon ECR
   ↓
Kubernetes / Amazon EKS
   ↓
OWASP ZAP DAST
   ↓
Runtime Verification & Monitoring
```

### Security Controls

* **SonarCloud** — Static Application Security Testing
* **Snyk** — Software Composition Analysis
* **Trivy** — Container image vulnerability scanning
* **OWASP ZAP** — Dynamic Application Security Testing
* **Jenkins Quality Gates** — Automated security and quality validation
* **Shift-Left Security** — Security integrated throughout the delivery lifecycle

---

# Docker & Containerization

Containerized applications across multiple technology stacks, including:

* Node.js / Express.js
* Java / Spring Boot
* Python / Django
* .NET
* Static websites

Hands-on Docker experience includes:

* Dockerfile development
* Image creation
* Dependency installation
* Container execution
* Port mapping
* Image management
* Container lifecycle operations
* Container troubleshooting
* Docker networking
* Persistent storage

Docker Compose experience includes:

* Two-tier WordPress applications
* Three-tier Kanban applications
* Multi-container networking
* Service dependencies
* Volumes
* Environment configuration
* Application troubleshooting

---

# Kubernetes & Amazon EKS

Hands-on Kubernetes experience includes deploying and operating containerized workloads on Amazon EKS.

### Experience includes

* EKS cluster provisioning with Terraform
* Kubernetes deployments
* Application replicas
* Kubernetes Services
* LoadBalancer services
* Amazon ECR image pulls
* Image digest verification
* Worker-node validation
* Application health validation
* `kubectl` operations
* Kubernetes troubleshooting
* Integration of Kubernetes deployment into CI/CD workflows

---

# Monitoring & Observability

Hands-on monitoring experience includes **Prometheus and Grafana**.

### Application Monitoring

* Prometheus-compatible application metrics
* Application health endpoints
* Runtime health verification
* Metrics collection

### Infrastructure & Kubernetes Monitoring

* Prometheus
* Grafana
* Kubernetes metrics
* Node-level monitoring
* Monitoring dashboards
* Service monitoring

The monitoring work demonstrates practical understanding of **observability, health checks, metrics collection, operational visibility, and post-deployment verification**.

---

# Application & Technology Experience

Hands-on development, deployment, and containerization experience across:

| Technology           | Experience                                        |
| -------------------- | ------------------------------------------------- |
| Node.js / Express.js | Application development, testing, Docker, CI/CD   |
| Java / Spring Boot   | Application development, Docker, CI/CD, DevSecOps |
| Python / Django      | Application deployment and containerization       |
| .NET                 | Application deployment and containerization       |
| Angular              | Frontend application in multi-tier architecture   |
| PostgreSQL           | Database in Docker Compose applications           |
| MySQL                | AWS RDS database                                  |
| HTML/CSS/JavaScript  | Static website development and deployment         |

### Testing

* Jest
* SuperTest
* Automated unit and application testing

---

# Security & Troubleshooting

Applied security and operational practices across the application and infrastructure lifecycle.

### Security

* IAM permissions
* AWS security groups
* SSH access controls
* SAST
* SCA
* Container vulnerability scanning
* DAST
* Kubernetes security considerations
* Shift-Left Security

### Troubleshooting

Hands-on troubleshooting has included:

* AWS networking and connectivity
* IAM permissions
* Terraform resource dependencies
* Terraform lifecycle issues
* Kubernetes resources
* LoadBalancer provisioning
* ECR repositories and images
* Jenkins configuration
* EKS connectivity
* Docker containers and networking
* CI/CD pipeline failures

I use verification and evidence-based troubleshooting to confirm that infrastructure, applications, security controls, containers, and deployment components are functioning as expected.

---

# Git, GitHub & Technical Documentation

Hands-on Git and GitHub experience includes:

* Repository management
* Version control
* Commits
* Pushes and updates
* Branching workflows
* Remote repository synchronization
* Project documentation

Technical documentation includes:

* Architecture
* Infrastructure configuration
* CI/CD pipelines
* Security controls
* Deployment procedures
* Verification results
* Troubleshooting procedures
* Implementation evidence

Detailed project documentation is maintained within the individual project repositories.

---

# Core Technology Stack

### Cloud

**AWS • EC2 • VPC • IAM • S3 • RDS • ECR • EKS • Elastic Load Balancing • Auto Scaling • AWS CLI**

### DevOps & CI/CD

**Jenkins • Git • GitHub • CI/CD • Continuous Integration • Continuous Delivery**

### Infrastructure & Automation

**Terraform • Ansible • Linux • Bash • Python**

### Containers & Orchestration

**Docker • Docker Compose • Kubernetes • Amazon EKS**

### DevSecOps

**SonarCloud • Snyk • Trivy • OWASP ZAP**

### Monitoring

**Prometheus • Grafana**

### Applications

**Node.js • Express.js • Java • Spring Boot • Python • Django • .NET • Angular • PostgreSQL • MySQL • HTML • CSS • JavaScript**

### Testing

**Jest • SuperTest**

---

# Professional Background

My transition into DevOps and Cloud Engineering builds on more than a decade of experience in **channel sales and business development**.

That background developed strong capabilities in:

* Customer and partner management
* Stakeholder communication
* Business requirements
* Problem-solving
* Cross-functional collaboration
* Market and competitive analysis
* Relationship management
* Commercial awareness

I now combine those capabilities with hands-on technical experience in **cloud infrastructure, automation, software delivery, security, containers, Kubernetes, monitoring, and Infrastructure as Code**.

This combination provides both a technical and business perspective when approaching technology, infrastructure, and operational challenges.

---

# Portfolio Summary

This portfolio represents an ongoing hands-on learning and implementation journey into **DevOps and Cloud Engineering**.

The projects demonstrate practical experience across the software and infrastructure lifecycle:

```text
Source Code
    ↓
Version Control
    ↓
Automated Testing
    ↓
Static Code Analysis
    ↓
Dependency Security
    ↓
Containerization
    ↓
Container Security
    ↓
Artifact Publishing
    ↓
Kubernetes Deployment
    ↓
Runtime Security
    ↓
Monitoring & Observability
    ↓
Verification & Troubleshooting
```

The goal is to continuously expand practical capability through **implementation, experimentation, troubleshooting, documentation, and evidence-based validation**.

**GitHub Portfolio:**
https://github.com/Jefferson-ohis1
