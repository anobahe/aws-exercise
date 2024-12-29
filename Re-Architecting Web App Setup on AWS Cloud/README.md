# Re-Architecting Web App Setup on AWS Cloud

This project demonstrates the process of re-architecting a dynamic Java web application to leverage the power of AWS Cloud for improved agility,
scalability, performance, and business continuity. By utilizing various AWS services. This project aims to provide a highly available and 
efficient infrastructure for hosting web applications.

## Key Objectives
- Refactoring the application to boost agility and improve business continuity.
- Adding new features and scaling effectively while ensuring good performance.

## AWS Services Used

### Elastic Beanstalk (PaaS)
Elastic Beanstalk simplifies application deployment and management by automatically handling the following:
- **EC2 Instances**: Virtual machines running Tomcat application servers.
- **Elastic Load Balancer**: Ensures high availability by distributing incoming traffic across multiple instances.
- **Auto Scaling**: Dynamically adjusts the number of instances based on load.
- **S3 Bucket**: Stores application artifacts.

### CloudWatch
Monitors the Auto Scaling group and triggers scale-in or scale-out actions based on performance metrics.

### RDS Instance
- **Database**: MySQL instance used for securely storing usernames and passwords.

### Amazon MQ (RabbitMQ)
- **Message Broker**: Acts as a middleman for communication between EC2 instances and the RDS database.

### Elastic Cache (Memcached)
- **Caching Layer**: Stores database query results to reduce latency and improve performance.

### Route 53
- **Domain Management**: Registers domain names and creates record sets for routing traffic.

### CloudFront
- **Content Delivery Network (CDN)**: Ensures low latency and fast content delivery for a global audience.

## Architecture Overview
The architecture includes the following components:
1. A web application deployed on Elastic Beanstalk, which automatically provisions and manages the necessary infrastructure.
2. A highly available MySQL database hosted on RDS for data persistence.
3. Amazon MQ as the messaging layer to decouple application components.
4. Memcached through Elastic Cache for caching database queries.
5. Route 53 for domain registration and traffic management.
6. CloudFront for optimizing content delivery across regions.

## Project Deliverables
1. **Reference Diagram**: A visual representation of the architecture setup.
2. **Screenshots**: Evidence of the successful deployment and functionality of the application hosted on Elastic Beanstalk.

Both the reference diagram and screenshots have been uploaded to the [GitHub repository](#) for this project.


This project demonstrates the seamless integration of AWS services to create a robust, scalable, and efficient environment for hosting Java web applications.

