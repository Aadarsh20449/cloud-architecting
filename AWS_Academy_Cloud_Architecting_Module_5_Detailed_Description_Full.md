
# AWS Academy Cloud Architecting - Module 5: Adding a Compute Layer Using Amazon EC2

## Module Overview

This module focuses on adding a compute layer using Amazon EC2. It details the key aspects of configuring EC2 instances, selecting instance types, managing storage, optimizing costs, and aligning with the AWS Well-Architected Framework.

---

### 1. Module Objectives
This module prepares you to:

- Use Amazon EC2 in a cloud architecture.
- Explain the value of Amazon Machine Images (AMIs) for creating and replicating infrastructure.
- Recommend EC2 instance types based on workloads.
- Recommend storage solutions for EC2.
- Configure instances with user data.
- Describe EC2 pricing models and recommend cost-efficient options.
- Launch an EC2 instance.
- Apply AWS Well-Architected Framework principles in designing EC2 architectures.

---

### 2. Adding Compute with Amazon EC2
Amazon EC2 provides virtual machines (VMs) in the cloud, offering flexible compute capacity. EC2 allows you to quickly provision instances, configure operating systems, and scale resources up or down based on demand.

---

### 3. Choosing an AMI (Amazon Machine Image)
An Amazon Machine Image (AMI) is a template used to launch EC2 instances. It includes the operating system, application stack, and any custom configurations.

#### Key Characteristics of AMIs:
- **Root Volume**: The volume containing the OS and initial software.
- **Launch Permissions**: Controls who can launch instances using the AMI.
- **Block Device Mappings**: Defines the additional storage volumes attached to the instance.

AMIs can be sourced from AWS (Quick Start), AWS Marketplace, custom-built, or community-shared.

---

### 4. Selecting an EC2 Instance Type
Choosing the right instance type is critical for optimizing performance and cost. An EC2 instance type defines CPU, memory, storage, and network characteristics.

#### Instance Type Categories:
- **General Purpose**: Balanced resources for most workloads. Example: M5, T3.
- **Compute Optimized**: For CPU-intensive tasks. Example: C5, C6.
- **Memory Optimized**: For memory-intensive applications. Example: R5, X1.
- **Storage Optimized**: High disk throughput. Example: I3, D2.
- **Accelerated Computing**: For workloads requiring hardware acceleration, such as AI or ML. Example: P3, G4.

Instance type names follow a naming convention (e.g., `c5.large`), where `c` represents compute optimized, `5` indicates the generation, and `.large` specifies the instance size.

---

### 5. Adding Storage to Amazon EC2
Amazon EC2 offers multiple storage options:

- **Instance Store**: Temporary block-level storage directly attached to the instance.
- **Amazon EBS (Elastic Block Store)**: Persistent block storage that can be attached/detached from instances.
- **Amazon EFS (Elastic File System)**: Network file system accessible by multiple instances.
- **Amazon FSx for Windows**: Fully managed Windows file server.

The root volume can be either EBS or Instance Store. EBS volumes are persistent and suitable for long-term storage. Instance Store is faster but non-persistent.

---

### 6. EC2 Pricing Models
Amazon EC2 provides several pricing options to help you manage costs efficiently:

- **On-Demand**: Pay-as-you-go with no long-term commitments.
- **Reserved Instances**: Save by committing to usage for 1 or 3 years.
- **Spot Instances**: Bid for unused EC2 capacity at lower prices.
- **Savings Plans**: Flexible pricing based on compute usage commitments.

You can also pay for Dedicated Hosts, where you use physical servers dedicated to your instances.

---

### 7. Configuring EC2 Instances with User Data
User data allows automation of configuration tasks during instance launch. You can pass scripts to install software or set up services automatically.

- **User Data**: Scripts executed during the instance’s boot process.
- **IAM Roles**: Attach roles to EC2 instances for secure API calls to AWS services.

---

### 8. Hands-on Labs
- **Guided Lab**: Introducing Amazon EFS – A step-by-step lab focused on integrating EFS with EC2.
- **Challenge Lab**: Creating a dynamic website using EC2 instances.

---

### 9. Key Takeaways
- Amazon EC2 offers flexibility in configuring virtual machines with different instance types and pricing models.
- AMIs simplify instance launch by providing reusable templates.
- Proper selection of instance types and storage solutions helps optimize performance and cost.
- User data and IAM roles enhance the security and automation of EC2 instances.
