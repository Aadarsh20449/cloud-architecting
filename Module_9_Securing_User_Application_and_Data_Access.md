
# AWS Academy Cloud Architecting: Module 9 - Securing User, Application, and Data Access

## Overview:
This module teaches how to secure access to AWS resources for users, applications, and data. It focuses on using AWS Identity and Access Management (IAM), AWS Key Management Service (KMS), and AWS security services for managing user identities, permissions, and data encryption.

---

## 1. **Managing Permissions**:
- **IAM Users, Groups, and Roles**: Manage user access by assigning permissions through policies. Instead of assigning permissions individually, use groups to simplify management.
- **Attribute-Based Access Control (ABAC)**: Uses attributes (tags) to define permissions, providing a scalable, flexible, and auditable approach. ABAC can replace traditional role-based access control (RBAC).
- **IAM Policies**: Policies are JSON documents that specify allowed or denied actions for users and roles.
  
---

## 2. **Federating Users**:
- **Identity Federation**: Allows users to access AWS resources using credentials from external identity providers (IdPs) like Facebook, Google, or corporate directories (using SAML or OpenID Connect).
- **AWS Services for Federation**: AWS IAM Identity Center and AWS STS enable federation and provide temporary credentials for users from federated IdPs.
  
---

## 3. **Managing Multiple Accounts**:
- **AWS Organizations**: A service that allows managing multiple AWS accounts centrally. Organizations provide consolidated billing and centralized security policies using Service Control Policies (SCPs).
- **SCPs**: Define guardrails for permissions across accounts to ensure compliance and control.
  
---

## 4. **Encrypting Data at Rest**:
- **AWS Key Management Service (KMS)**: Used to create and manage cryptographic keys to encrypt data at rest. AWS KMS integrates with several AWS services to protect sensitive data.
- **Envelope Encryption**: Encrypts data keys using another key, creating layers of security for data at rest.
- **Symmetric vs Asymmetric Encryption**: Symmetric encryption uses one key for both encryption and decryption, while asymmetric encryption uses a public-private key pair for added security.

---

## 5. **AWS Security Services**:
- AWS offers services like Amazon Cognito for securing application access by providing authentication and authorization mechanisms, as well as SSO capabilities.

---
