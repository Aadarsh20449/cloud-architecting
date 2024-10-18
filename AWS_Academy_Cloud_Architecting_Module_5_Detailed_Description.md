
# AWS Academy Cloud Architecting - Module 5: Adding a Compute Layer Using Amazon EC2

## Module Overview

This module covers how to add a compute layer to cloud architectures using Amazon EC2. It explores various aspects like instance types, storage options, configuration, and pricing models for using EC2.

---

### 1. Introduction to Amazon EC2
Amazon EC2 provides virtual machines (VMs) in the cloud with flexible options to run various workloads. It offers resizable compute capacity, supports a variety of operating systems, and can be launched within minutes. It helps you scale up or down based on demand and pay only for what you use.

---

### 2. AWS Runtime Compute Choices
- **VMs (Amazon EC2)**: Provides secure and resizable compute capacity in the cloud.
- **Containers (Amazon ECS/EKS)**: Docker containers on AWS.
- **VPS (Amazon Lightsail)**: Simplified virtual private servers with predictable pricing.
- **PaaS (AWS Elastic Beanstalk)**: Service to automatically manage the deployment of web applications.
- **Serverless (AWS Lambda/Fargate)**: Execute code without managing servers.

---

### 3. EC2 Virtualization and Instances
Amazon EC2 uses virtualization technology to run instances (VMs) on physical hosts. Instances run on an AWS hypervisor, and you can select different configurations (CPU, memory, storage) depending on your needs.

#### EC2 Instance Lifecycle:
- **Launch (pending state)**: The instance is being provisioned.
- **Running**: The instance is active and can be connected to.
- **Stop/Start**: Stop and start an instance without data loss (for EBS-backed instances).
- **Terminate**: Shut down and delete the instance.

---

### 4. Choosing an AMI (Amazon Machine Image)
An AMI is a template that contains software configurations (OS, applications). It helps launch EC2 instances with consistent environments.
- **Sources of AMIs**: AWS Marketplace, Quick Start, My AMIs, and Community AMIs.
- **Root Device Types**: Amazon EBS-backed (persistent) or instance store-backed (temporary).

---

### 5. EC2 Instance Types and Workloads
- **General Purpose**: Balanced CPU, memory, and networking. Examples: M7, M6, T4, T3.
- **Compute Optimized**: For compute-heavy workloads like HPC. Examples: C7, C6.
- **Memory Optimized**: For memory-intensive applications. Examples: R6, X1.
- **Storage Optimized**: For high-performance storage workloads. Examples: I3, D2.
- **Accelerated Computing**: For machine learning and AI workloads. Examples: P5, G5.

---

### 6. Adding Storage to Amazon EC2
Amazon EC2 instances use a root volume and can have additional data volumes.
- **Instance Store**: Temporary, high-speed block storage.
- **Amazon EBS (Elastic Block Store)**: Persistent block storage that can be detached and reattached to instances.
- **Amazon EFS (Elastic File System)**: Network file system accessible by multiple instances (Linux).
- **Amazon FSx for Windows**: Managed file system for Windows workloads.

---

### 7. EC2 Pricing Models
- **On-Demand Instances**: Pay by the hour or second with no long-term commitments.
- **Reserved Instances**: Save up to 75% by committing to a 1- or 3-year term.
- **Spot Instances**: Bid for unused EC2 capacity at significant discounts.
- **Savings Plans**: Flexible pricing model offering savings based on compute usage.

---

### 8. Hands-on Labs and Activities
This module includes a guided lab on **Amazon EFS** and a challenge lab for creating a dynamic website architecture using EC2. It also includes an activity for selecting appropriate EC2 instance types for various workloads.

---

### Key Takeaways
- Amazon EC2 provides virtual machines in the cloud that offer flexibility, scalability, and multiple purchasing options.
- Choosing the correct instance type, AMI, and storage solution is critical to optimizing performance and costs.
- Using lifecycle management, security groups, and IAM roles enhances EC2 instance security and operations.
