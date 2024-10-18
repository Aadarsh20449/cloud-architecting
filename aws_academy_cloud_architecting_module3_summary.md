
# AWS Academy Cloud Architecting Module 3: "Securing Access"

## 1. Introduction to Securing Access
The module focuses on security principles and concepts related to securing access to AWS cloud resources. Key topics include the AWS shared responsibility model, AWS Identity and Access Management (IAM), and best practices for access control and data protection.

## 2. AWS Shared Responsibility Model
The model outlines the division of security responsibilities between AWS and its customers:
- **AWS responsibility (Security OF the Cloud)**: AWS manages the infrastructure, including the physical security of data centers and hardware.
- **Customer responsibility (Security IN the Cloud)**: Customers are responsible for securing their applications, data, network configurations, and managing identity and access.

## 3. Security Pillar of the AWS Well-Architected Framework
The security pillar of the AWS Well-Architected Framework emphasizes best practices, including:
- **Implementing a strong identity foundation** (e.g., IAM, multi-factor authentication).
- **Protecting data in transit and at rest** using encryption.
- **Applying security at all layers** with a defense-in-depth approach.
- **Maintaining traceability** with real-time monitoring and auditing.
- **Automating security best practices** to scale securely.
  
## 4. Principle of Least Privilege
A critical principle of cloud security, least privilege means granting only the permissions necessary for users to perform their tasks. Start with minimal permissions and add more as needed, while revoking unnecessary permissions over time.

## 5. Encrypting Data in Transit and at Rest
- **Data in transit**: Protected through encryption protocols like TLS, securing data as it moves between networks.
- **Data at rest**: Protected through encryption, with options for client-side and server-side encryption (e.g., AWS services like S3 provide server-side encryption).

## 6. AWS Identity and Access Management (IAM)
IAM enables fine-grained access control to AWS resources, supporting:
- **Users, groups, roles**: IAM roles provide temporary security credentials, while users and groups manage access levels.
- **Policies**: IAM policies define access permissions and are attached to users, groups, and roles. Identity-based policies and resource-based policies help fine-tune access control.

## 7. Best Practices for Securing Access
Key best practices include:
- **Enforcing least privilege** by granting minimal necessary permissions.
- **Enabling multi-factor authentication (MFA)** to add an extra layer of security.
- **Using temporary credentials** for human users and rotating long-term credentials.
- **Securing root user** by using it only for essential tasks and protecting it with MFA.

## 8. IAM Policies and Permissions
IAM policies define permissions using JSON documents. Policies include:
- **Effect**: Allow or Deny.
- **Action**: Specifies the actions allowed (e.g., s3:GetObject).
- **Resource**: Defines the resources affected by the policy.
IAM evaluates policies to determine access: an explicit allow overrides the default deny, but an explicit deny always overrides an allow.

## 9. Role-Based Access
IAM roles provide temporary security credentials for applications, services, or users, making them useful for granting cross-account or federated access. Roles are not associated with long-term credentials, enhancing security by reducing reliance on static keys.

## 10. Hands-on Lab: Exploring IAM
The module includes a lab where students practice creating and managing IAM policies, assigning users to groups, and using IAM sign-in URLs.

## 11. Module Summary
Students learned to describe security principles in the AWS Cloud, explain the purpose of IAM users, groups, and roles, and understand how IAM policies determine access permissions in AWS accounts.

---

This module covers the foundational aspects of securing access in AWS cloud environments, emphasizing the shared responsibility model, IAM, encryption practices, and the principle of least privilege. By following these practices, architects can secure cloud resources effectively and ensure compliance with organizational policies.
