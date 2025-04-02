
# Section 1: Introduction to cloud computing
#### What is cloud computing?
Cloud computing is the on-demand delivery of compute power, database, storage, applications, and other IT resources via the internet with pay-as-you-go pricing.

#### Traditional computing model
- Infrastructure as hardware
- Hardware solutions:
	- Require space, staff, physical security, planning, capital expenditure
	- Have a long hardware procurement cycle
	- Require you to provision capacity by guessing theoretical maximum peaks

### Cloud service models
![Pasted image 20250328141858](https://github.com/user-attachments/assets/8d3f111d-4e84-490a-a485-ca9d79a12080)

#### 1. **Infrastructure as a Service (IaaS)**

- **Definition**: Provides virtualized computing resources over the internet. Users manage the OS, applications, and runtime while the provider manages the underlying infrastructure.
- **Examples**: AWS EC2, Google Compute Engine, Microsoft Azure Virtual Machines.
- **Use Cases**: Hosting websites, data storage, running custom applications, and disaster recovery.
#### 2. **Platform as a Service (PaaS)**

- **Definition**: Provides a platform with tools and services to develop, test, and deploy applications. Users focus on development while the provider manages the infrastructure, OS, and runtime.
- **Examples**: AWS Elastic Beanstalk, Google App Engine, Microsoft Azure App Services.
- **Use Cases**: Application development, database management, and container orchestration.

#### 3. **Software as a Service (SaaS)**

- **Definition**: Delivers fully managed applications over the internet. Users interact with the software without worrying about maintenance, infrastructure, or security.
- **Examples**: Gmail, Google Drive, Microsoft Office 365, Dropbox.
- **Use Cases**: Email services, file storage, customer relationship management (CRM), and collaboration tools.


### Cloud computing deployment models
![Pasted image 20250328142752](https://github.com/user-attachments/assets/dc700b72-401a-4e9a-9cf1-ccfabf972c3c)

---
---

# Section 2: Advantages of cloud computing

#### 1- Trade capital expense for variable expense
replace large upfront capital expenses (CapEx) with variable operational expenses (OpEx)

#### 2-Massive economies of scale
Because of aggregate usage from all customers, AWS can achieve higher economies of scale and pass savings on to customers

#### 3- Stop guessing capacity
Eliminate guessing about your infrastructure capacity needs.

#### 4- Increase speed and agility
enabling businesses to innovate faster and respond to changes more effectively.
#### 5- Stop spending money on running and maintaining data centers

#### 6- Go global in minutes

___
---
# Section 3: Introduction to Amazon Web Services (AWS)

#### What are web services?
![Pasted image 20250328143718](https://github.com/user-attachments/assets/3209fd5b-fcab-44d5-afca-e62afbb52ddf)


### AWS Services
![Pasted image 20250328143921](https://github.com/user-attachments/assets/efe67fc5-27bd-4247-a48b-c7e84e3c253c)


### Three ways to interact with AWS
![Pasted image 20250328144059](https://github.com/user-attachments/assets/abcbfb4b-c83a-4326-9830-dd27c69e0e5c)

---
# Section 4: Moving to the AWS Cloud –The AWS Cloud Adoption Framework (AWS CAF)


The ==**AWS Cloud Adoption Framework (AWS CAF)**== helps organizations **accelerate cloud adoption** by providing **structured guidance** across key business and technical areas. It identifies **six key perspectives** that help organizations **plan, migrate, and optimize** their cloud journey.

![Pasted image 20250328145431](https://github.com/user-attachments/assets/007c61ac-0930-4bf4-a173-a77df08960bb)

#### 1️⃣ **Business**

- Aligns cloud adoption with **business goals**.
- Focuses on financial benefits, agility, and market opportunities.
- Example: **Reducing IT costs by 30% using AWS Reserved Instances**.
#### 2️⃣ **People**

- Manages **organizational change and workforce readiness**.
- Ensures teams have the right **skills and training** for cloud operations.
- Example: **AWS Training & Certification for DevOps engineers**.
#### 3️⃣ **Governance**

- Defines **policies, compliance, and risk management**.
- Establishes **financial controls and security guidelines**.
- Example: **AWS Control Tower for multi-account governance**.

#### 4️⃣ **Platform**

- Covers **cloud architecture, infrastructure, and DevOps automation**.
- Ensures **scalability, reliability, and cost optimization**.
- Example: **Using AWS Well-Architected Framework for best practices**.

#### 5️⃣ **Security**

- Focuses on **identity management, data protection, and compliance**.
- Uses AWS security services like **IAM, KMS, GuardDuty, and WAF**.
- Example: **Implementing AWS IAM roles for least privilege access**.

#### 6️⃣ **Operations**

- Defines **monitoring, incident response, and continuous improvement**.
- Uses **AWS CloudWatch, AWS Config, and AWS X-Ray** for insights.    
- Example: **Automating alerts with AWS CloudWatch Alarms**.

---

# Sample exam question


1- Which of the following is an advantage that the AWS Cloud provides to users?  
==A. Users eliminate the need to guess about infrastructure capacity requirements.  ==
B. Users decrease their variable costs by maintaining sole ownership of IT hardware.  
C. Users maintain control of underlying IT infrastructure hardware.  
D. Users maintain control of operating systems for managed services.  
Correct Answer: A

2- Which of the following are advantages of moving to the AWS Cloud? (Choose two.)  
A. Users can implement all AWS services in seconds.  
B. AWS assumes all responsibility for the security of infrastructure and applications.  
==C. Users experience increased speed and agility.  
D. Users benefit from massive economies of scale. ==
E. Users can move hardware from their data center to the AWS Cloud.  
Correct Answer: CD


3- Which of the following are advantages of moving from on premises to the AWS Cloud? (Choose two.)  
A. Trade variable expenses for capital expenses.  
==B. Eliminate costs related to running and maintaining data centers.  
C. Benet from massive economies of scale==.  
D. Eliminate the need to tram IT staff.  
E. Gam the ability to reserve capacity for 7 years or more.  
Correct Answer: CB

4- Which of the following are advantages of moving to the AWS Cloud? (Choose two.)  
A. The ability to turn over the responsibility for all security to AWS  
==B. The ability to use the pay as you go model  ==
C. The ability to have full control over the physical infrastructure  
==D. No longer having to guess what capacity will be required  ==
E. No longer worrying about users access controls  
Correct Answer: BD

5- Which of the following is an advantage of AWS Cloud computing?  
A. Trade security for elasticity  
B. Trade operational excellence for agility  
==C. Trade fixed expenses for variable expenses==
D. Trade elasticity for performance  
Correct Answer: C

6- Which of the following are advantages of the AWS Cloud? (Choose two.)  
A. AWS manages all the security within the cloud.  
B. Expenses never change from month to month.  
==C. Users can stop spending money on the maintenance of data centers.  ==
D. Users do not need to deploy applications globally.  
==E. Users can stop guessing about resource capacity.  ==
Correct Answer: CE

7- Which abilities are benefits of the AWS Cloud? (Choose two.)  
A. Trade variable expenses for capital expenses.  
==B. Deploy globally in minutes.  ==
C. Plan capacity in advance of deployments.  
==D. Take advantage of economies of scale.==
E. Reduce dependencies on network connectivity.  
Correct Answer: BD

8- Which option is an AWS Cloud Adoption Framework (AWS CAF) perspective?  
A. Cloud uency  
==B. Security==
C. Change acceleration  
D. Architecture  
Correct Answer: B

9- A company is planning its migration to the AWS Cloud. The company is identifying its capability gaps by using the AWS Cloud Adoption  
Framework (AWS CAF) perspectives.  
Which phase of the cloud transformation journey includes these identication activities?  
A. Envision  
==B. Align  ==
C. Scale  
D. Launch  
Correct Answer: B

10- Which options are common stakeholders for the AWS Cloud Adoption Framework (AWS CAF) platform perspective? (Choose two.)  
A. Chief nancial ocers (CFOs)  
==B. IT architects  ==
C. Chief information ocers (CIOs)  
D. Chief data ocers (CDOs)  
==E. Engineers  ==
Correct Answer: BE

11- A company wants to migrate its applications to the AWS Cloud. The company plans to identify and prioritize any business transformation  
opportunities and evaluate its AWS Cloud readiness.  
Which AWS service or tool should the company use to meet these requirements?  
==A. AWS Cloud Adoption Framework (AWS CAF)  ==
B. AWS Managed Services (AMS)  
C. AWS Well-Architected Framework  
D. AWS Migration Hub  
Correct Answer: A

12- A company is planning to migrate to the AWS Cloud. The company is conducting organizational transformation and wants to become more  
responsive to customer inquiries and feedback.  
Which tasks should the company perform to meet these requirements, according to the AWS Cloud Adoption Framework (AWS CAF)? (Choose  
two.)  
==A. Realign teams to focus on products and value streams.==
B. Create new value propositions with new products and services.  
==C. Use agile methods to rapidly iterate and evolve==
D. Use a new data and analytics platform to create actionable insights.  
E. Migrate and modernize legacy infrastructure
Correct Answer: AC


