
# AWS Academy Cloud Architecting - Module 4: Adding a Storage Layer with Amazon S3

## 1. Amazon S3 Overview
- **What is Amazon S3?**: Amazon Simple Storage Service (Amazon S3) is an object storage service designed to store and retrieve any amount of data from anywhere. It offers high scalability, security, and performance.
- **How does it work?**: Amazon S3 stores data as "objects" in "buckets". Each object is assigned a unique key and can be accessed via a globally unique URL. S3 allows virtually unlimited storage capacity.
- **Object Details**: Objects contain data, metadata, and a globally unique URL. Object sizes range from 0 bytes to 5 TB.

## 2. Types of Storage
- **Block Storage**: Data is stored in fixed-sized blocks, suitable for file systems and databases.
- **File Storage**: Data is stored in a hierarchical structure, commonly used for shared file systems.
- **Object Storage (S3)**: S3 uses object storage, where objects are stored with metadata and scaled horizontally.

## 3. Amazon S3 Use Cases
- **Hosting Media Content**: Ideal for hosting videos, photos, and other media. It can also serve as the origin for content delivery networks (CDNs) like Amazon CloudFront.
- **Static Website Hosting**: S3 can host static websites (HTML, images, client-side scripts) without a web server.
- **Data Backup and Recovery**: Long-term data backup and disaster recovery, with cross-region replication options.
- **Analytics**: S3 stores raw and processed data for computational workloads, which can be analyzed with tools like Amazon QuickSight.

## 4. Moving Data to and from S3
- **Uploading Objects**: Use the AWS Management Console, CLI, SDKs, or REST API to upload objects.
- **Multipart Upload**: For large files, multipart uploads improve speed and allow recovery from network issues.
- **S3 Transfer Acceleration**: Speeds up long-distance uploads by routing them through CloudFront edge locations.

## 5. Storing Content in S3
- **Storage Classes**: S3 offers several storage classes for balancing cost and performance, including:
  - **S3 Standard**: For frequently accessed data.
  - **S3 Intelligent-Tiering**: Automatically moves objects between tiers based on access frequency.
  - **S3 Glacier**: For long-term archival storage.
- **Lifecycle Policies**: Define rules to transition objects between storage classes or delete them after a specific period.
- **Versioning**: Protects against accidental overwrites or deletions by maintaining multiple versions of an object.

## 6. Security and Encryption
- **Default Security**: All S3 buckets and objects are private by default. Server-side encryption (SSE) is used to secure objects at rest.
- **IAM Policies**: Control access using IAM policies, bucket policies, and access control lists (ACLs).
- **Cross-Origin Resource Sharing (CORS)**: Configure CORS to allow web applications from one domain to access resources in another domain.

This module prepares you to use Amazon S3 effectively, considering use cases, access patterns, security best practices, and cost optimization.

For hands-on practice, the module includes activities such as:
- Setting up a static website on Amazon S3.
- Managing S3 lifecycle rules and versioning.
