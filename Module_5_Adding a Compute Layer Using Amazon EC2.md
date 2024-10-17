# AWS Academy Cloud Architecting: Module 5 - Adding a Compute Layer Using Amazon EC2

## Overview
This module covers the use of Amazon Elastic Compute Cloud (EC2) for building and optimizing compute layers in AWS architectures. Key topics include launching EC2 instances, selecting Amazon Machine Images (AMIs), instance types, storage options, and applying AWS Well-Architected Framework principles.

## Key Topics

### 1. Amazon EC2 Overview
- Virtual machines in the cloud with scalable, resizable compute capacity.
- Support for multiple OS including Linux and Windows.
- **Pay-as-you-go** model, with flexibility to scale.

### 2. Amazon Machine Images (AMIs)
- **AMIs** are templates used to launch EC2 instances.
- Includes the root volume, launch permissions, and block device mappings.
- AMIs ensure repeatability and reusability for consistent infrastructure deployment.

### 3. Instance Types
- **Instance types** define configurations for CPU, memory, storage, and network performance.
- **Types of instance families**:
  - General Purpose (M5, T3)
  - Compute Optimized (C5)
  - Memory Optimized (R5)
  - Storage Optimized (I3)
  - Accelerated Computing (P3)

### 4. EC2 Storage
- **Amazon EBS**: Persistent storage for EC2 instances, supporting SSD and HDD-backed volumes.
  - **SSD-backed volumes**: Ideal for IOPS-heavy workloads.
  - **HDD-backed volumes**: Suitable for throughput-heavy workloads.
- **Instance Store**: Temporary storage tied to the lifecycle of the EC2 instance.

### 5. EC2 Pricing Options
- **On-Demand Instances**: Flexible, pay for what you use.
- **Reserved Instances**: Discounted rates for long-term commitment (1-3 years).
- **Spot Instances**: Purchase unused capacity at reduced prices.

### 6. Launching an EC2 Instance
- Steps: Choose an AMI, select instance type, configure security (key pair and security group), add storage, and configure network settings.

### 7. AWS Well-Architected Framework
- Ensures that EC2 deployments align with the pillars of operational excellence, security, reliability, performance efficiency, and cost optimization.

## Labs
- Hands-on labs in this module include launching EC2 instances, configuring storage, and optimizing compute resources.

## Conclusion
Amazon EC2 offers a highly flexible and scalable compute solution for a variety of workloads, from small websites to large-scale machine learning applications. Selecting the right instance type and pricing model ensures efficient use of AWS resources.
