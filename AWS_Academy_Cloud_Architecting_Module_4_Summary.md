
# AWS Academy Cloud Architecting - Module 4: Adding a Storage Layer with Amazon S3

## Module Overview

This module covers various aspects of adding a storage layer with Amazon S3 in cloud architectures. The focus is on defining S3, its components, use cases, data transfer methods, lifecycle management, and security features.

---

### 1. Introduction to Amazon S3
Amazon S3 is introduced as a service designed for object storage that stores massive amounts of unstructured data in a scalable, highly durable, and available manner. The data is stored in objects within buckets. Key benefits include high durability (11 nines), availability (99.99%), and performance that scales automatically.

---

### 2. Amazon S3 Storage Types
- **Block storage**: Stores data in fixed-sized blocks.
- **File storage**: Stores data in a hierarchical structure.
- **Object storage**: Stores data as objects (composed of data, metadata, and a unique object key). S3 is an object storage service.

---

### 3. Amazon S3 Components
- **Buckets**: Containers for objects with globally unique names.
- **Objects**: Files stored in S3, uniquely identified by an object key and optional version ID.
- **Metadata**: Data describing the object, including system-assigned and user-defined metadata.

---

### 4. Amazon S3 Use Cases
- **Media hosting**: Store and distribute video, music, and image files.
- **Static websites**: Host websites composed of static content.
- **Data for computation**: Store data that can be processed and analyzed using tools like Amazon EMR or QuickSight.
- **Backup and disaster recovery**: Store backup data or archives, with optional cross-region replication for higher durability.

---

### 5. Data Transfer to/from S3
- **Data upload methods**:
  - AWS Management Console (up to 160 GB)
  - AWS CLI and SDKs (useful for programmatic access)
  - REST API
  - **Multipart uploads** for large files (>100 MB) to improve upload speeds and resiliency.
  
- **S3 Transfer Acceleration**: Uses CloudFront edge locations to speed up data transfer over long distances.
  
- **AWS Transfer Family**: Facilitates secure file transfers using standard protocols like SFTP, FTPS, and FTP into S3 or EFS.

---

### 6. Storage Classes in S3
- **S3 Standard**: For frequently accessed data.
- **S3 Intelligent-Tiering**: Automatically moves data between access tiers based on usage.
- **S3 Standard-IA (Infrequent Access)**: For data that is accessed less frequently.
- **S3 Glacier**: Archival storage with millisecond retrieval (Instant), or asynchronous (Flexible Retrieval).
- **S3 Glacier Deep Archive**: Lowest-cost option for long-term data retention.

---

### 7. Lifecycle Management
Lifecycle policies allow automatic transition of data between different storage classes or deletion of objects after a set period. These policies help optimize cost by moving older or less accessed data to cheaper storage options.

---

### 8. Versioning
Versioning protects objects by keeping multiple versions within a bucket. This helps recover from accidental deletes or overwrites. With versioning enabled, each object gets a unique version ID.

---

### 9. Security in S3
S3 provides several layers of security:
- **Default Encryption**: Server-side encryption with S3-managed keys (SSE-S3) is enabled by default.
- **IAM Policies**: Control access to buckets and objects.
- **Bucket Policies**: Manage access based on specific conditions.
- **Access Control Lists (ACLs)**: An older method for setting access, generally less preferred than IAM policies.
- **Block Public Access**: Prevents public access to S3 buckets.
- **CORS**: Allows cross-origin resource sharing for web applications accessing S3 resources.

---

### 10. Amazon S3 Data Consistency
Amazon S3 provides **strong read-after-write consistency**, which ensures that once a PUT request is completed, subsequent reads will return the latest version of the object. This simplifies big data workloads and analytics.

---

### 11. Cost Structure
- **Storage cost**: Charged by the size of the data stored and the selected storage class.
- **Request costs**: PUT, COPY, and GET requests are priced per operation.
- **Data transfer costs**: Free for data transferred within the same region and to CloudFront.

---

### 12. Hands-On Lab
The module includes a hands-on lab that focuses on creating a static website using Amazon S3 and managing access for employees to certain documents, aligning with real-world business needs.

---

### Key Takeaways
- Amazon S3 is an object storage solution offering durability, availability, and scalability.
- Use S3 for media hosting, data backups, and as part of large-scale analytics.
- Security and encryption mechanisms are essential for protecting data.
- Lifecycle policies and versioning are crucial for optimizing storage costs and managing data efficiently.
