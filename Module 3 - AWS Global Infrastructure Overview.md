
# Section 1: AWS Global Infrastructure



AWS operates a **highly available, secure, and scalable cloud infrastructure** across the world. It consists of:  
**Regions**  
 **Availability Zones (AZs)**  
 **Edge Locations & Points of Presence (PoPs)**

### **1 AWS Regions** 

-  AWS Region is a geographical area.
	- Data replication across Regions is controlled by you.
	- Communication between Regions uses AWS backbone network infrastructure.
- Each Region provides full redundancy and connectivity to the network.
- A Region typically consists of three or more Availability Zones

### **2 AWS Availability Zones (AZs)** 

- Each Region has multiple Availability Zones.
- Each Availability Zone is a fully isolated partition of the AWS infrastructure.
	- Availability Zones consist of discrete data centers
	- They are designed for fault isolation
	- They are interconnected with other Availability Zones by using high-speed private networking
	- You choose your Availability Zones.
	- AWS recommends replicating data and resources across Availability Zones for resiliency
	- Availability Zones have their own power infrastructure, and they are physically separated by many kilometers from other Availability Zones—though all Availability Zones are within 100 km of each other.



### **3 AWS data centers
- AWS data centers are designed for security.
- Data centers are where the data resides and data processing occurs.
- Each data center has redundant power, networking, and connectivity, and is housed in a separate facility.
- A data center typically has 50,000 to 80,000 physical servers.



### **4️ AWS Edge Locations & Points of Presence (PoPs)** 

- AWS provides a global network of Points of Presence locations 
- Consists of edge locations and a much smaller number of Regional edge caches
- Used with Amazon CloudFront 
- A global Content Delivery Network (CDN), that delivers content to end users with reduced latency
- Regional edge caches used for content with infrequent access.

![[Pasted image 20250329112524.png]]


#### **Content Delivery Network (CDN) in AWS** 

- A **Content Delivery Network (CDN)** is a globally distributed system of servers that helps **deliver web content, videos, APIs, and applications** faster by caching data at **edge locations** near users.

- AWS provides **Amazon CloudFront**, a highly scalable **CDN service** that speeds up content delivery with **low latency and high security**.

---
---

# Section 2: AWS services and service category overview

### AWS foundational services
![[Pasted image 20250329114316.png]]

### Storage service category

-  ==Amazon Simple Storage Service (Amazon S3)== is an object storage service that offers scalability, data availability, security, and performance. Use it to store and protect any amount of data for websites, mobile apps, backup and restore, archive, enterprise applications, Internet of Things (IoT) devices, and big data analytics. 

- ==Amazon Elastic Block Store (Amazon EBS)== is high-performance block storage that is designed for use with Amazon EC2 for both throughput and transaction intensive workloads. It is used for a broad range of workloads, such as relational and non-relational databases, enterprise applications, containerized applications, big data analytics engines, file systems, and media workflows.

- ==Amazon Elastic File System (Amazon EFS)== provides a scalable, fully managed elastic Network File System (NFS) file system for use with AWS Cloud services and on-premises resources. It is built to scale on demand to petabytes, growing and shrinking automatically as you add and remove files. It reduces the need to provision and manage capacity to accommodate growth.

- ==Amazon Simple Storage Service Glacier== is a secure, durable, and extremely low-cost Amazon S3 cloud storage class for data archiving and long-term backup. It is designed to deliver 11 9s of durability, and to provide comprehensive security and compliance capabilities to meet stringent regulatory requirements

---
### Compute service category

- ==Amazon Elastic Compute Cloud (Amazon EC2)== provides resizable compute capacity as virtual machines in the cloud.
-
- ==Amazon EC2 Auto Scaling== enables you to automatically add or remove EC2 instances according to conditions that you define. 

- ==Amazon Elastic Container Service (Amazon ECS==) is a highly scalable, high-performance container orchestration service that supports Docker containers. 

- ==Amazon Elastic Container Registry (Amazon ECR)== is a fully-managed Docker container registry that makes it easy for developers to store, manage, and deploy Docker container images. 

- ==AWS Elastic Beanstalk== is a service for deploying and scaling web applications and services on familiar servers such as Apache and Microsoft Internet Information Services (IIS). 

- ==AWS Lambda== enables you to run code without provisioning or managing servers. You pay only for the compute time that you consume. There is no charge when your code is not running.

- ==Amazon Elastic Kubernetes Service (Amazon EKS)== makes it easy to deploy, manage, and scale containerized applications that use Kubernetes on AWS.

- ==AWS Fargate== is a compute engine for Amazon ECS that allows you to run containers without having to manage servers or clusters


---

### Database service category

- ==Amazon Relational Database Service (Amazon RDS)== makes it easy to set up, operate, and scale a relational database in the cloud. It provides resizable capacity while automating time-consuming administration tasks such as hardware provisioning, database setup, patching, and backups. 

- ==Amazon Aurora== is a MySQL and PostgreSQL-compatible relational database. It is up to five times faster than standard MySQL databases and three times faster than standard PostgreSQL databases.

- ==Amazon Redshift ==enables you to run analytic queries against petabytes of data that is stored locally in Amazon Redshift, and directly against exabytes of data that are stored in Amazon S3. It delivers fast performance at any scale.

- ==Amazon DynamoDB== is a key-value and document database that delivers single-digit millisecond performance at any scale, with built-in security, backup and restore, and in-memory caching

---
### Networking and content delivery service category

- ==Amazon Virtual Private Cloud (Amazon VPC)== enables you to provision logically isolated sections of the AWS Cloud. Elastic Load Balancing automatically distributes incoming application traffic across multiple targets, such as Amazon EC2 instances, containers, IP addresses, and Lambda functions.

- ==Amazon CloudFront== is a fast content delivery network (CDN) service that securely delivers data, videos, applications, and application programming interfaces (APIs) to customers globally, with low latency and high transfer speeds.

- ==AWS Transit Gateway== is a service that enables customers to connect their Amazon Virtual Private Clouds (VPCs) and their on-premises networks to a single gateway.

- ==Amazon Route 53== is a scalable cloud Domain Name System (DNS) web service designed to give you a reliable way to route end users to internet applications. It translates names (like www.example.com) into the numeric IP addresses (like 192.0.2.1) that computers use to connect to each other. 

- ==AWS Direct Connect== provides a way to establish a dedicated private network connection from your data center or office to AWS, which can reduce network costs and increase bandwidth throughput.

- ==AWS VPN== provides a secure private tunnel from your network or device to the AWS global network.

---
### Security, identity, and compliance service category

- ==AWS Identity and Access Management (IAM==) enables you to manage access to AWS services and resources securely. By using IAM, you can create and manage AWS users and groups. You can use IAM permissions to allow and deny user and group access to AWS resources. 

- ==AWS Organizations== allows you to restrict what services and actions are allowed in your accounts. 

- ==Amazon Cognito== lets you add user sign-up, sign-in, and access control to your web and mobile apps.

- ==AWS Artifact== provides on-demand access to AWS security and compliance reports and select online agreements. 

- ==AWS Key Management Service (AWS KMS)== enables you to create and manage keys. You can use AWS KMS to control the use of encryption across a wide range of AWS services and in your applications.

- ==AWS Shield== is a managed Distributed Denial of Service (DDoS) protection service that safeguards applications running on AWS


---
### AWS cost management service category

- ==AWS Cost and Usage Report== contains the most comprehensive set of AWS cost and usage data available, including additional metadata about AWS services, pricing, and reservations.

- ==AWS Budgets== enables you to set custom budgets that alert you when your costs or usage exceed (or are forecasted to exceed) your budgeted amount.

- ==AWS Cost Explorer== has an easy-to-use interface that enables you to visualize, understand, and manage your AWS costs and usage over time

---
### Management and governance service category

- ==AWS Management Console== provides a web-based user interface for accessing your AWS account.
- ==AWS Config== provides a service that helps you track resource inventory and changes.
- ==Amazon CloudWatch ==allows you to monitor resources and applications.
- ==AWS Auto Scaling== provides features that allow you to scale multiple resources to meet demand.
- ==AWS Command Line Interface== provides a unified tool to manage AWS services.
- ==AWS Trusted Advisor== helps you optimize performance and security.
- ==AWS Well-Architected== Tool provides help in reviewing and improving your workloads.
- ==AWS CloudTrail== tracks user activity and API usage.
---
---




# Sample exam question

1- Which tasks are the responsibility of AWS, according to the AWS shared responsibility model? (Choose two.)  
A. Patch the Amazon EC2 guest operating system.  
==B. Upgrade the firmware of the network infrastructure.  ==
C. Apply password rotation for IAM users.  
==D. Maintain the physical security of edge locations.  ==
E. Maintain least privilege access to the root user account.  
Correct Answer: BD


2- Which AWS service uses edge locations?  
A. Amazon Aurora  
==B. AWS Global Accelerator  ==
C. Amazon Connect  
D. AWS Outposts  
Correct Answer: B


3- Which of the following does Amazon CloudFront use to distribute content to users around the world?  
A. Amazon VPC  
B. AWS Local Zones  
==C. Edge locations  ==
D. Availability Zones  
Correct Answer: C


4- A company wants its Amazon EC2 instances to share the same geographic area but use multiple independent underlying power sources.  
Which solution achieves this goal?  
A. Use EC2 instances in a single Availability Zone.  
B. Use EC2 instances in multiple AWS Regions.  
==C. Use EC2 instances in multiple Availability Zones in the same AWS Region.  ==
D. Use EC2 instances in the same edge location and the same AWS Region.  
Correct Answer: C


5- A company wants to set up a secure network connection from on premises to the AWS Cloud within 1 week.  
Which solution will meet these requirements?  
A. AWS Direct Connect  
B. Amazon VPC  
==C. AWS Site-to-Site VPN  ==
D. Edge location  
Correct Answer: C



6- Which AWS service or feature provides high availability and low latency within an AWS Region?  
A. Edge locations  
==B. Availability Zones  ==
C. AWS Outposts  
D. Amazon Route 53  
Correct Answer: B



7- A company has deployed an application in the AWS Cloud. The company wants to ensure that the application is highly resilient.  
Which component of AWS infrastructure can the company use to meet this requirement?  
A. Content delivery network (CDN)  
B. Edge locations  
C. Wavelength Zones  
==D. Availability Zones  ==
Correct Answer: D


8- Which AWS service offers a global content delivery network (CDN) that helps companies securely deliver websites, videos, applications, and APIs  
at high speeds with low latency?  
A. Amazon EC2  
==B. Amazon CloudFront  ==
C. Amazon CloudWatch  
D. AWS CloudFormation  
Correct Answer: B

9- A company is running its application in the AWS Cloud and wants to protect against a DDoS attack. The company’s security team wants near realtime visibility into DDoS attacks.  
Which AWS service or trac lter will meet these requirements with the MOST features for DDoS protection?  
==A. AWS Shield Advanced  ==
B. AWS Shield  
C. Amazon GuardDuty  
D. Network ACLs  
Correct Answer: A



10- A company needs to identify who accessed an AWS service and what action was performed for a given time period.  
Which AWS service should the company use to meet this requirement?  
A. Amazon CloudWatch  
==B. AWS CloudTrail  ==
C. AWS Security Hub  
D. Amazon Inspector  
Correct Answer: B

11- Which AWS service, feature, or tool helps visualize the pattern of AWS spending?  
==A. Cost Explorer  ==
B. Amazon DevPay  
C. AWS CloudTrail  
D. Consolidated billing  
Correct Answer: A

12- A company wants to securely store Amazon RDS database credentials and automatically rotate user passwords periodically.  
Which AWS service or capability will meet these requirements?  
A. Amazon S3  
B. AWS Systems Manager Parameter Store  
==C. AWS Secrets Manager  ==
D. AWS CloudTrail  
Correct Answer: C


13- What are some advantages of using Amazon EC2 instances to host applications in the AWS Cloud instead of on premises? (Choose two.)  
A. EC2 includes operating system patch management.  
==B. EC2 integrates with Amazon VPC, AWS CloudTrail, and AWS Identity and Access Management (IAM).  ==
C. EC2 has a 1 00% service level agreement (SLA).  
==D. EC2 has a exible, pay-as-you-go pricing model.  ==
E. EC2 has automatic storage cost optimization.  
Correct Answer: BD

14- A security engineer wants a single-tenant AWS solution to create, control, and manage their own cryptographic keys to meet regulatory  
compliance requirements for data security.  
Which AWS service should the engineer use?  
A. AWS Key Management Service (AWS KMS)  
B. AWS Certicate Manager (ACM)  
==C. AWS CloudHSM  ==
D. AWS Systems Manager  
Correct Answer: C


15- A company is designing an identity access management solution for an application. The company wants users to be able to use their social  
media, email, or online shopping accounts to access the application.  
Which AWS service provides this functionality?  
A. AWS IAM Identity Center (AWS Single Sign-On)  
B. AWS Cong  
==C. Amazon Cognito  ==
D. AWS Identity and Access Management (IAM)  
Correct Answer: C

16- A company needs a solution that can provide automated notifications and perform automated actions if the company’s monthly AWS costs  
exceed a specific threshold.  
Which AWS service or tool provides this functionality?  
==A. AWS Budgets  ==
B. AWS Cost Explorer  
C. AWS Trusted Advisor  
D. Amazon Inspector  
Correct Answer: A

17- A company needs to securely store important credentials that an application uses to connect users to a database.  
Which AWS service can meet this requirement with the MINIMAL amount of operational overhead?  
A. AWS Key Management Service (AWS KMS)  
B. AWS Cong  
==C. AWS Secrets Manager  ==
D. Amazon GuardDuty  
Correct Answer: C

















