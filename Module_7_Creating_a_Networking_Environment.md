
# AWS Academy Cloud Architecting: Module 7 - Creating a Networking Environment

## Overview:
This module focuses on how to create and configure a networking environment using Amazon Virtual Private Cloud (VPC) and related AWS services. It discusses how to isolate resources, secure them, and monitor your network in AWS.

---

## 1. **Amazon VPC Basics**:
Amazon Virtual Private Cloud (VPC) is a logically isolated virtual network that you can define within an AWS region. It allows you to control the networking environment, including private IP addresses, subnets, route tables, and internet gateways. Key concepts include:
- **CIDR Blocks**: Defines the size of your VPC based on the range of IP addresses.
- **Subnets**: Dividing your VPC into smaller, more manageable sections.
- **Internet Gateway**: Allows resources in public subnets to access the internet.
  
---

## 2. **Network Security**:
AWS recommends using **security layers** to protect your resources. 
- **Security Groups**: Stateful firewalls for instances, controlling traffic at the resource level.
- **Network ACLs (Access Control Lists)**: Stateless firewalls controlling traffic at the subnet level.
- **NAT Gateway**: Allows private subnet resources to access the internet without being exposed to inbound internet traffic.

---

## 3. **Public and Private Subnets**:
Resources in a **public subnet** are directly accessible from the internet, while resources in a **private subnet** are isolated and only accessible through other internal AWS services or private connections.

---

## 4. **Connecting to AWS Services**:
- **VPC Endpoints**: Connect your VPC privately to supported AWS services like Amazon S3 and DynamoDB.
- **Interface VPC Endpoints (PrivateLink)**: Used for secure communication with AWS services via private IPs.
- **Gateway VPC Endpoints**: Directly connect to AWS services like Amazon S3.

---

## 5. **Monitoring Your Network**:
- **VPC Flow Logs**: Capture and monitor traffic to and from your VPC for troubleshooting.
- **Reachability Analyzer**: Tests the connectivity between two resources in your VPC.
- **Traffic Mirroring**: Copies network traffic for deeper analysis.

---

## 6. **AWS Well-Architected Framework**:
This module also integrates the **AWS Well-Architected Framework** principles, emphasizing:
- **Reliability**: Ensure IP subnet allocation accounts for future expansion.
- **Security**: Apply Zero Trust principles by controlling traffic at all layers.
- **Performance Efficiency**: Understand the impact of network configurations on workload performance.
- **Cost Optimization**: Select the best AWS regions and network designs for cost efficiency.

---
