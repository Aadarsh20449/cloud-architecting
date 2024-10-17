
# AWS Academy Cloud Architecting - Module 5: Adding a Database Layer

## 1. Database Layer Considerations
When designing a database layer, several key considerations are important:
- **Scalability**: Ensure the database can handle the required throughput and scale as needed.
- **Storage Requirements**: Determine the size of the database in terms of gigabytes, terabytes, or more.
- **Data Characteristics**: Understand the data model and access patterns.
- **Durability**: Ensure data durability, availability, and recoverability, especially for critical data.

## 2. Relational and Non-Relational Databases
- **Relational Databases**: Structured data stored in tables with strict schema rules, often optimized for transactional use cases (OLTP).
- **Non-Relational Databases (NoSQL)**: Flexible schemas, designed for fast access to structured, semi-structured, or unstructured data.

## 3. Amazon RDS (Relational Database Service)
- **Amazon RDS Overview**: A fully managed relational database service that supports multiple database engines (MySQL, PostgreSQL, MariaDB, Oracle, SQL Server).
- **Benefits of Amazon RDS**: Reduces administrative burden, scales easily, offers high availability, and provides security features like encryption.
- **Use Cases**: Suitable for applications like transactional databases, ERP systems, and CRM platforms.

## 4. Amazon DynamoDB (NoSQL Database)
- **Overview**: A fully managed, serverless NoSQL database that supports key-value and document data models.
- **Use Cases**: Ideal for high-concurrency applications like gaming platforms, media stores, and real-time applications.
- **Features**: Offers encryption by default, point-in-time recovery, and multi-region, multi-active replication.

## 5. Purpose-Built Databases
AWS offers several purpose-built databases optimized for specific use cases:
- **Amazon DocumentDB**: For document data models.
- **Amazon Redshift**: For data warehousing.
- **Amazon Neptune**: For graph databases.
- **Amazon Timestream**: For time-series data.
- **Amazon Quantum Ledger Database (QLDB)**: For ledger applications.
  
## 6. Database Migration
- **Migration Options**: AWS provides tools for migrating on-premises databases to the cloud, including AWS Database Migration Service (DMS).
- **Strategies**: Plan for minimal downtime and seamless data transfer during migration.

## 7. Security and Encryption
- **Best Practices**: Use IAM for access control, encrypt data at rest and in transit, and use VPC for network isolation.
