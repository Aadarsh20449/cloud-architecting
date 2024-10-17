
# AWS Academy Cloud Architecting: Module 8 - Connecting Networks

## Overview:
This module focuses on how to connect Virtual Private Clouds (VPCs) and on-premises networks to AWS. It covers AWS services like AWS Transit Gateway, VPC Peering, Site-to-Site VPN, and AWS Direct Connect, and how to use them to create a scalable, secure, and efficient network infrastructure.

---

## 1. **Scaling your VPC network with AWS Transit Gateway**:
- **AWS Transit Gateway** is a centralized, regional router that connects multiple VPCs and on-premises networks in a hub-and-spoke architecture. 
- It automatically scales based on traffic and can be peered with other transit gateways across AWS regions. Transit Gateway Flow Logs help in monitoring traffic.
- It reduces complexity compared to full mesh architectures and simplifies management of many VPCs.

---

## 2. **Connecting VPCs in AWS with VPC Peering**:
- **VPC Peering** creates a point-to-point network connection between two VPCs, allowing private network communication between them.
- It's a low-cost option for smaller networks and offers low latency but doesn’t support transitive peering, meaning traffic doesn’t automatically pass between other peered VPCs.
- You can use VPC peering for VPCs in different AWS accounts and regions.

---

## 3. **Connecting to your remote network with AWS Site-to-Site VPN**:
- **Site-to-Site VPN** provides a secure IPsec connection between an on-premises network and a VPC, using two VPN tunnels for high availability. 
- It’s a quick way to connect an on-premises network to AWS, with dynamic and static routing options available based on the customer gateway.

---

## 4. **Connecting to your remote network with AWS Direct Connect**:
- **AWS Direct Connect** offers a private, dedicated connection from an on-premises network to AWS. It bypasses the public internet, offering consistent performance and higher bandwidth.
- It’s ideal for hybrid environments with large data sets or applications requiring predictable performance.
  
---

## 5. **Applying AWS Well-Architected Framework to Network Connectivity**:
- AWS recommends using best practices from the **Well-Architected Framework** to ensure your network is reliable, secure, and cost-effective.
- Principles include provisioning redundant connections, using hub-and-spoke topologies, and ensuring encryption for data in transit.

---
