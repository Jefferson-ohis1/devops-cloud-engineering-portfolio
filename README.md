# DevOps & Cloud Engineering — Hands-on Project Portfolio

## Portfolio Overview

This portfolio documents my hands-on transition into **DevOps and Cloud Engineering**, with practical projects covering AWS cloud infrastructure, Infrastructure as Code (IaC), CI/CD, DevSecOps, containerization, Kubernetes, automation, networking, monitoring, and troubleshooting.

My project-based approach emphasizes **designing, implementing, securing, deploying, validating, documenting, and troubleshooting** applications and infrastructure across AWS and local development environments.

The portfolio complements my background in channel sales and business development with technical problem-solving, automation, security awareness, cross-functional collaboration, and business understanding.

## Technical Focus

- ☁️ **Cloud Engineering:** AWS, EC2, VPC, IAM, S3, RDS, ECR, EKS, Load Balancing, Auto Scaling
- 🏗️ **Infrastructure as Code:** Terraform
- ⚙️ **Automation:** Ansible, Bash, Linux, Python
- 🔄 **CI/CD:** Jenkins, GitHub Actions, Git, GitHub, automated testing
- 🔐 **DevSecOps:** Gitleaks, SonarCloud, Snyk, Trivy, OWASP ZAP
- 🐳 **Containers:** Docker, Docker Compose
- ☸️ **Orchestration:** Kubernetes, Amazon EKS, Helm
- 📊 **Observability:** Prometheus, Grafana, application metrics, health checks
- 🧪 **Testing:** Jest, SuperTest
- 🔧 **Operations:** AWS CLI, kubectl, infrastructure validation, troubleshooting

---

# Featured Projects

## 1. End-to-End Node.js CI/CD & DevSecOps Platform on AWS

**Primary project repository:** [End-to-End Node.js CI/CD & DevSecOps Platform](https://github.com/Jefferson-ohis1/end-to-end-node-ci-cd-devsecops)

Designed, implemented, and documented an end-to-end DevSecOps platform for a Node.js monitoring application across 11 documented phases. The project progressed from application testing and Docker containerization to cloud infrastructure, two CI/CD implementations, security governance, Kubernetes deployment, observability, autoscaling, and infrastructure teardown.

### Technologies

**AWS • Terraform • Jenkins • GitHub Actions • GitHub OIDC • Node.js • Express • Jest • SuperTest • Docker • Amazon ECR • Amazon EKS • Kubernetes • Helm • Gitleaks • SonarCloud • Snyk • Trivy • OWASP ZAP • Prometheus • Grafana**

### Key Capabilities

- Tested a Node.js/Express application with Jest and SuperTest.
- Containerized the application using a multi-stage Docker build and a non-root runtime user.
- Provisioned AWS infrastructure using Terraform, including resources for networking, IAM, Amazon ECR, and Amazon EKS.
- Implemented Jenkins-based CI/CD and subsequently developed GitHub Actions as a **second CI/CD implementation**, not a replacement for Jenkins.
- Integrated automated code, dependency, container-image, and web-application security validation using SonarCloud, Snyk, Trivy, and OWASP ZAP.
- Implemented pull-request validation and repository governance with Gitleaks secret detection, branch protection, and required status checks.
- Configured GitHub Actions authentication to AWS using OIDC and a dedicated IAM role, avoiding reliance on long-lived AWS access keys in the workflow.
- Published container images to Amazon ECR and deployed the application to Amazon EKS.
- Managed Kubernetes Metrics Server separately using Terraform and Helm to support the Kubernetes Metrics API and Horizontal Pod Autoscaler (HPA).
- Verified application health, resource metrics, Kubernetes deployment behaviour, and HPA scale-up and scale-down behaviour.
- Documented implementation phases, architecture decisions, screenshots, verification results, and release evidence.
- Published the final implementation as `v0.11.0 — Phase 11: Complete DevSecOps Platform` and destroyed the temporary AWS environment after validation.

### Architecture Evolution

The project evolved from a Jenkins-centred delivery implementation to a more clearly separated application-delivery and platform-management model.

**Jenkins implementation:** GitHub → Jenkins → automated testing and security validation → Docker → Amazon ECR → Amazon EKS.

Prometheus and Grafana were used during the Jenkins implementation, with the monitoring stack hosted on the Jenkins server.

**GitHub Actions implementation:** GitHub → GitHub Actions → AWS OIDC/IAM → Amazon ECR and Amazon EKS.

The Kubernetes Metrics Server dependency was managed separately through Terraform and Helm, supporting the Kubernetes Metrics API and HPA.

This evolution demonstrates practical work across CI/CD automation, security integration, cloud identity, infrastructure management, Kubernetes operations, and evidence-driven validation.

### Project Resources

- [Main project repository](https://github.com/Jefferson-ohis1/end-to-end-node-ci-cd-devsecops)
- [Project case study](https://github.com/Jefferson-ohis1/end-to-end-node-ci-cd-devsecops/blob/main/docs/portfolio/01-project-case-study.md)
- [Project presentation — PowerPoint](https://github.com/Jefferson-ohis1/end-to-end-node-ci-cd-devsecops/blob/main/docs/portfolio/02-project-presentation.pptx)
- [Portfolio summary](https://github.com/Jefferson-ohis1/end-to-end-node-ci-cd-devsecops/blob/main/docs/portfolio/03-portfolio-summary.md)

---

## 2. Java DevSecOps CI/CD Pipeline

**Repository:** [Java DevSecOps CI/CD Pipeline](https://github.com/Jefferson-ohis1/java-devsecops-ci-cd-pipeline)

Built a Jenkins-based delivery pipeline for a Java 17/Spring Boot application using Maven and Docker in an AWS EC2 environment.

### Technologies

**Java 17 • Spring Boot • Maven • Jenkins • Docker • AWS EC2 • SonarCloud • Snyk • Trivy • OWASP ZAP**

### Key Capabilities

- Automated application build and delivery through Jenkins.
- Containerized the application using Docker.
- Integrated SonarCloud for source-code analysis.
- Integrated Snyk for dependency vulnerability analysis.
- Used Trivy for container-image vulnerability scanning.
- Used OWASP ZAP Baseline Scan for dynamic web-application security testing.
- Published Docker images and archived security reports as pipeline evidence.

**Detailed implementation:** See the repository for pipeline configuration, security controls, implementation details, and supporting documentation.

---

## 3. AWS Infrastructure with Terraform

**Repository:** [Infrastructure as Code — Terraform](https://github.com/Jefferson-ohis1/Infrastructure-as-code-Terraform)

Practised provisioning and managing AWS infrastructure through repeatable, version-controlled Terraform configurations.

### AWS Resources and Concepts

- Amazon VPC and subnet configuration
- Public and private networking
- Route tables and Internet Gateways
- Security groups
- IAM roles and permissions
- Amazon EC2
- Amazon ECR
- Amazon EKS
- Infrastructure dependencies and resource lifecycle management

### Practical Experience

- Terraform configuration and infrastructure provisioning
- Resource dependency management
- Infrastructure verification
- Terraform state management
- AWS networking and connectivity troubleshooting
- Infrastructure destruction and lifecycle troubleshooting

---

## 4. Automated Nginx Website Deployment with Ansible

**Repository:** [Ansible Nginx Static Website Deployment](https://github.com/Jefferson-ohis1/Ansible-nginx-static-website-deployment)

Implemented repeatable website deployment and configuration management across AWS EC2 instances.

### Technologies

**Ansible • AWS EC2 • Linux • Nginx • SSH**

### Key Capabilities

- Inventory and playbook configuration
- Automated Nginx installation and configuration
- Service start-up and enablement
- Static website deployment
- Multi-host automation
- SSH-based remote execution
- Deployment verification

---

## 5. Three-Tier Kanban Application with Docker Compose

**Repository:** [Three-Tier Kanban Application](https://github.com/Jefferson-ohis1/Using-Docker-compose-To-Deploy-A-Three-Tier-App-Kanban-App)

Deployed a multi-container application demonstrating communication between frontend, backend, and database tiers.

### Architecture

```text
Angular Frontend
       |
       v
Java / Spring Boot Backend
       |
       v
PostgreSQL Database
```

### Technologies

**Angular • Java • Spring Boot • PostgreSQL • Docker • Docker Compose**

### Key Capabilities

- Multi-container application architecture
- Docker image creation and execution
- Docker Compose orchestration
- Container networking and port mapping
- Service dependencies
- PostgreSQL persistent storage
- Application configuration
- Multi-tier troubleshooting

---

## 6. WordPress Two-Tier Application with Docker Compose

**Repository:** [WordPress Two-Tier Application](https://github.com/Jefferson-ohis1/Using-Docker-compose-To-Deploy-A-Two-Tier-App-WordPress-App)

Deployed a containerized WordPress application with a separate database service using Docker Compose.

### Key Capabilities

- WordPress and database containerization
- Docker Compose orchestration
- Container networking
- Environment configuration
- Persistent storage and volumes
- Service dependencies
- Multi-container troubleshooting

---

# AWS Cloud & Infrastructure Experience

My hands-on AWS projects cover cloud resource provisioning, configuration, access management, networking, deployment, verification, and troubleshooting.

### Compute

- Amazon EC2
- Linux server configuration
- SSH access and security groups
- Launch Templates
- Auto Scaling Groups
- HTTP application access and verification

### Networking

- Amazon VPC
- Public and private subnets
- Route tables and Internet Gateways
- Security groups
- Load Balancers
- Network traffic flow and connectivity troubleshooting

### Storage and Databases

- Amazon S3 object management
- Static website hosting
- Cross-region replication practice
- Amazon RDS for MySQL

### Identity and Security

- AWS IAM users, groups, roles, and permissions
- Access controls and least-privilege considerations
- EC2 access controls
- SSH access
- GitHub OIDC authentication to AWS

### Containers and Kubernetes

- Amazon ECR image publishing and verification
- Amazon EKS
- Kubernetes workloads and Services
- Application deployment and rollout verification
- Kubernetes Metrics Server and resource metrics
- Horizontal Pod Autoscaler validation

### AWS Operations and Cost Awareness

- AWS CLI
- Resource inspection and configuration verification
- Authentication and authorization troubleshooting
- AWS Cost Explorer
- AWS Budgets
- Basic cloud cost monitoring and budgeting

**Environment note:** The flagship DevSecOps project was validated in a temporary AWS environment that was subsequently destroyed. The repositories and documentation provide the implementation details and evidence; the project should not be interpreted as a permanently hosted live service.

---

# Infrastructure as Code & Automation

## Terraform

Used Terraform to provision and manage AWS infrastructure through repeatable, version-controlled configurations.

Practical work includes:

- AWS networking and IAM
- EC2, ECR, and EKS infrastructure
- Resource dependencies
- Terraform state and lifecycle management
- Infrastructure validation
- Troubleshooting provisioning and destruction issues

Terraform was also used alongside Helm to manage the Kubernetes Metrics Server platform dependency separately from the application-delivery workflow.

## Ansible

Used Ansible for configuration management and automated deployment across AWS EC2 instances.

Practical work includes:

- Inventory management
- Playbook development
- Nginx installation and service configuration
- Website deployment
- Multi-host automation
- Deployment verification

---

# CI/CD & DevSecOps

My hands-on pipeline work covers both Node.js and Java applications, using Jenkins and GitHub Actions for automated delivery workflows.

## Jenkins CI/CD

The Jenkins implementation integrates application testing, security validation, container-image creation, artifact publishing, Kubernetes deployment, and post-deployment checks.

```text
GitHub
   |
   v
Jenkins
   |
   v
Automated Testing
   |
   v
SonarCloud / Snyk
   |
   v
Docker Build
   |
   v
Trivy Image Scan
   |
   v
Amazon ECR
   |
   v
Amazon EKS
   |
   v
Deployment Verification
   |
   v
OWASP ZAP / Runtime Checks
```

## GitHub Actions CI/CD

GitHub Actions provides a second application-delivery implementation for the flagship Node.js project.

The workflow includes automated testing, Docker image building, AWS authentication through OIDC, ECR image publishing, and EKS deployment verification.

The workflow uses a dedicated AWS IAM role and temporary credentials rather than relying on long-lived AWS access keys stored in GitHub Actions.

## DevSecOps Governance

The flagship project includes pull-request validation and repository governance controls designed to prevent unvalidated changes from entering the delivery workflow.

Controls include:

- Gitleaks secret detection
- Automated tests
- SonarCloud source-code analysis
- Snyk dependency analysis
- Trivy container-image scanning
- OWASP ZAP web-application testing
- Pull-request-based change control
- Branch protection and required status checks

These controls demonstrate the integration of security validation and change governance into the delivery process.

---

# Docker & Containerization

Containerized applications across multiple technology stacks, including Node.js/Express, Java/Spring Boot, Python/Django, .NET, and static websites.

### Docker Experience

- Dockerfile development
- Image creation and management
- Container execution and lifecycle operations
- Port mapping and networking
- Dependency installation
- Persistent storage
- Container troubleshooting

### Docker Compose Experience

- Two-tier WordPress applications
- Three-tier Kanban applications
- Multi-container networking
- Service dependencies
- Volumes and environment configuration
- Application troubleshooting

The flagship Node.js project also uses a multi-stage Docker build and a non-root runtime user.

---

# Kubernetes & Amazon EKS

Hands-on Kubernetes work includes deploying and validating containerized workloads on Amazon EKS.

### Experience Includes

- EKS cluster provisioning with Terraform
- Kubernetes Deployments and replicas
- Kubernetes Services and LoadBalancer services
- Amazon ECR image integration
- Image and rollout verification
- Worker-node validation
- Application health checks
- `kubectl` operations and troubleshooting
- Kubernetes deployment integration with CI/CD
- Horizontal Pod Autoscaler configuration and behaviour verification

### Platform Metrics and Autoscaling

The flagship project separates application delivery from the Metrics Server platform dependency.

Terraform and Helm manage Metrics Server, which supplies resource metrics through the Kubernetes Metrics API for use by the HPA controller.

Observed HPA behaviour during validation included scaling from two replicas to four, then five, and back to two replicas.

This demonstrated functional autoscaling behaviour rather than simply confirming the existence of an HPA resource.

---

# Monitoring & Observability

Hands-on monitoring work includes application metrics, Prometheus, Grafana, health checks, Kubernetes resource metrics, and post-deployment verification.

### Application Monitoring

- Prometheus-compatible application metrics
- Application health endpoints
- Runtime health verification
- Metrics collection

### Monitoring Tools and Platform Metrics

- Prometheus
- Grafana
- Kubernetes resource metrics
- Metrics Server and the Kubernetes Metrics API
- Monitoring dashboards
- Service and workload monitoring

During the Jenkins implementation, a Prometheus stack was hosted on the Jenkins server, with Grafana used for visualization. The later GitHub Actions design managed the Kubernetes Metrics Server dependency separately through Terraform and Helm.

This work demonstrates practical understanding of observability, operational visibility, health checks, metrics collection, and runtime validation.

---

# Application Technologies & Testing

My projects include hands-on refactoring, deployment, testing, and containerization across several application stacks.

| Technology | Project experience |
|---|---|
| Node.js / Express | Application refactoring, Jest/SuperTest, Docker, CI/CD, metrics |
| Java / Spring Boot | Application delivery, Maven, Docker, Jenkins, DevSecOps |
| Python / Django | Application deployment and containerization practice |
| .NET | Application deployment and containerization practice |
| Angular | Frontend in a multi-tier application |
| PostgreSQL | Database in a Docker Compose application |
| MySQL | AWS RDS database practice |
| HTML / CSS / JavaScript | Static website development and deployment |

### Testing Tools

- **Jest:** Automated application testing
- **SuperTest:** HTTP endpoint and application integration testing

Testing and validation are incorporated into the delivery workflow to help verify application behaviour before deployment.

---

# Security & Troubleshooting

Applied security and operational practices across application delivery, cloud infrastructure, and containerized workloads.

### Security Practices

- AWS IAM permissions and access controls
- Security groups and SSH access controls
- Source-code analysis
- Dependency vulnerability analysis
- Container-image vulnerability scanning
- Dynamic web-application security testing
- Secret detection
- Pull-request validation and repository governance
- OIDC-based AWS authentication for GitHub Actions
- Kubernetes security considerations

### Troubleshooting Experience

Hands-on troubleshooting has included:

- AWS networking and connectivity
- IAM permissions and authorization
- Terraform resource dependencies and lifecycle issues
- Kubernetes resources and cluster connectivity
- LoadBalancer provisioning
- ECR repositories and container images
- Jenkins configuration and CI/CD failures
- Docker containers and networking
- Application health and deployment verification
- Kubernetes resource metrics and HPA behaviour

My approach emphasizes evidence-based troubleshooting: inspect the configuration, reproduce or observe the behaviour, validate the correction, and document the result.

---

# Git, GitHub & Technical Documentation

Used Git and GitHub to manage project source code, configuration, workflows, and technical documentation.

### Version Control and Repository Practices

- Repository management
- Version control and commits
- Branching and change management
- Remote repository synchronization
- Pull-request workflows and repository governance
- Git history and release management

### Documentation and Evidence

Project documentation includes:

- Architecture and design decisions
- Infrastructure configuration
- CI/CD pipeline definitions
- Security controls
- Deployment procedures
- Verification results
- Troubleshooting guidance
- Screenshots and implementation evidence
- Release documentation

The flagship project follows an evidence-driven workflow:

```text
Implement
   |
   v
Build
   |
   v
Verify
   |
   v
Capture Evidence
   |
   v
Document
   |
   v
Commit and Push
```

---

# Core Technology Stack

**Cloud:** AWS, EC2, VPC, IAM, S3, RDS, ECR, EKS, Elastic Load Balancing, Auto Scaling, AWS CLI

**DevOps & CI/CD:** Jenkins, GitHub Actions, Git, GitHub, CI/CD

**Infrastructure & Automation:** Terraform, Ansible, Linux, Bash, Python, Helm

**Containers & Orchestration:** Docker, Docker Compose, Kubernetes, Amazon EKS

**DevSecOps:** Gitleaks, SonarCloud, Snyk, Trivy, OWASP ZAP

**Monitoring & Observability:** Prometheus, Grafana, application metrics, Metrics Server

**Applications:** Node.js, Express.js, Java, Spring Boot, Python, Django, .NET, Angular, PostgreSQL, MySQL, HTML, CSS, JavaScript

**Testing:** Jest, SuperTest

---

# Professional Background

My transition into DevOps and Cloud Engineering builds on more than a decade of experience in **channel sales and business development**.

That background developed capabilities in:

- Customer and partner management
- Stakeholder communication
- Business requirements and commercial priorities
- Cross-functional collaboration
- Market and competitive analysis
- Negotiation and relationship management
- Problem-solving and business awareness

I now combine those capabilities with hands-on technical work in cloud infrastructure, automation, software delivery, security, containers, Kubernetes, monitoring, and Infrastructure as Code.

This combination provides both technical and business perspectives when approaching technology and operational challenges.

---

# Portfolio Resources

Explore the portfolio and supporting technical materials:

- **[GitHub Profile](https://github.com/Jefferson-ohis1)** — repositories and project work
- **[Flagship Node.js CI/CD & DevSecOps Project](https://github.com/Jefferson-ohis1/end-to-end-node-ci-cd-devsecops)** — implementation, phase documentation, configuration, and evidence
- **[AWS DevSecOps Project Case Study](https://github.com/Jefferson-ohis1/end-to-end-node-ci-cd-devsecops/blob/main/docs/portfolio/01-project-case-study.md)** — project objectives, architecture, implementation, validation, and lessons learned
- **[End-to-End DevSecOps Platform — Project Presentation](https://github.com/Jefferson-ohis1/end-to-end-node-ci-cd-devsecops/blob/main/docs/portfolio/02-project-presentation.pptx)** — visual project walkthrough
- **[Portfolio Summary](https://github.com/Jefferson-ohis1/end-to-end-node-ci-cd-devsecops/blob/main/docs/portfolio/03-portfolio-summary.md)** — concise overview of the flagship project
- **[Java DevSecOps CI/CD Pipeline](https://github.com/Jefferson-ohis1/java-devsecops-ci-cd-pipeline)** — Java-based delivery and security pipeline
- **[Terraform AWS Infrastructure](https://github.com/Jefferson-ohis1/Infrastructure-as-code-Terraform)** — Infrastructure as Code project

---

# Portfolio Summary

This portfolio demonstrates hands-on project work across the software delivery and cloud infrastructure lifecycle.

```text
Source Code
    |
    v
Version Control
    |
    v
Automated Testing
    |
    v
Security Validation
    |
    v
Containerization
    |
    v
Artifact Publishing
    |
    v
Kubernetes Deployment
    |
    v
Observability and Autoscaling
    |
    v
Verification and Troubleshooting
    |
    v
Documentation and Release
    |
    v
Infrastructure Cleanup
```

The goal is to continue developing practical capability through implementation, experimentation, troubleshooting, documentation, and evidence-based validation.

**GitHub Portfolio:** [github.com/Jefferson-ohis1](https://github.com/Jefferson-ohis1)