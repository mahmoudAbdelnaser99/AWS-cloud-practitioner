
# Section 1: Fundamentals of pricing

#### AWS pricing model
Three fundamental drivers of cost with AWS
![[Pasted image 20250328154155.png]]

#### How do you pay for AWS?
![[Pasted image 20250328154331.png]]

#### 1- Pay for what you use
Pay only for the services that you consume, with no large upfront expenses

#### 2- pay less when you reserve
Invest in Reserved Instances (RIs):
- Save up to 75 percent
- Options:
	- All Upfront Reserved Instance (==AURI==) →largest discount
	- Partial Upfront Reserved Instance (==PURI==) →lower discounts
	- No Upfront Payments Reserved Instance (==NURI==) →smaller discount
#### 3- Pay less by using more
Realize volume-based discounts:
- Savings as usage increases.
- Tiered pricing for services like Amazon Simple Storage Service (Amazon S3), Amazon Elastic Block Store (Amazon EBS), or Amazon Elastic File System (Amazon EFS) →the more you use, the less you pay per GB.
- Multiple storage services deliver lower storage costs based on needs

#### 4- Pay even less as AWS grows
- AWS focuses on lowering cost of doing business.
- This practice results in AWS passing savings from economies of scale to you.
- Since 2006, AWS has lowered pricing 75times (as of September 2019).
- Future higher-performing resources replace current resources for no extra charge
#### 5- Custom pricing
- Meet varying needs through custom pricing.
- Available for high-volume projects with unique requirements.

### Services with no charge
![[Pasted image 20250328163555.png]]

---
---
# Section 2: Total Cost of Ownership

**Total Cost of Ownership (TCO)** is the financial estimate to help identify direct and indirect costs of a system.

**Why use TCO?**
- To compare the costs of running an entire infrastructure environment or specific workload on-premises versus on AWS
- To budget and build the business case for moving to the cloud

### TCO considerations
![[Pasted image 20250328164010.png]]


## AWS Pricing Calculator
![[Pasted image 20250328164407.png]]



---
---

# Section 3: AWS Organizations
AWS Organizations is a service that helps businesses **centrally manage** and **govern multiple AWS accounts**. It allows for **consolidated billing, policy enforcement, and security controls** across an enterprise’s AWS environment.

### AWS Organizations terminology
![[Pasted image 20250328171155.png]]
 An OU is a container for accounts within a root. An OU can also contain other OUs .This structure enables you to create a hierarchy that looks like an upside-down tree with the root at the top. The branches consist of child OUs and they move downward until they end in accounts, which are like the leaves of the tree


#### AWS Organizations enables you to:
- Create **service control policies (SCPs)** that centrally control AWS services across multiple AWS accounts.•
- Create **groups of accounts** and then attach policies to a group to ensure that the correct policies are applied across the accounts.
- Simplify account management by using **application programming interfaces (APIs)** to automate the creation and management of new AWS accounts.
- Simplify the billing process by setting up a single payment method for all the AWS accounts in your organization. With **consolidated billing**, you can see a combined view of charges that are incurred by all your accounts, and you can take advantage of pricing benefits from aggregated usage. Consolidated billing provides a central location to manage billing across all of your AWS accounts, and the ability to benefit from volume discounts


### Security with AWS Organizations
![[Pasted image 20250328171815.png]]


#### Limits of AWS Organizations
![[Pasted image 20250328172017.png]]



---
---
# Section 4: AWS Billing and Cost Management 

AWS **Billing and Cost Management** is a set of tools that help businesses **track, manage, and optimize** their AWS expenses. It ensures transparency and helps organizations **control costs** effectively.

#### **AWS Cost Management Tools**

|**Tool**|**Purpose**|
|---|---|
|**AWS Cost Explorer**|Helps visualize spending trends and forecast costs.|
|**AWS Budgets**|Allows users to set spending limits and receive alerts.|
|**AWS Cost and Usage Report (CUR)**|Provides detailed cost and usage data in CSV format.|
|**AWS Compute Optimizer**|Suggests ways to optimize EC2, Lambda, and other compute services.|
|**AWS Savings Plans & Reserved Instances (RI)**|Helps reduce costs for long-term workloads.|

==The Cost Explorer== is a free tool that enables you to:
- View charts of your costs.
- View cost data for the past 13 months.
- Forecast how much you are likely to spend over the next 3 months.
- Discover patterns in how much you spend on AWS resources over time and identify cost problem areas.
- Identify the services that you use the most
- View metrics, like which Availability Zones have the most traffic or which linked AWS account is used the most

==AWS Budgets & Alerts==

-  **Set budgets for overall spending, services, or accounts.**  
- **Receive alerts via email or SNS when spending exceeds limits.**  
- **Track reserved instance utilization & coverage.**


---
# Section 5: Technical support 

### **AWS Support Plans & Features**

|**Support Plan**|**Best For**|**Key Features**|**Cost**|
|---|---|---|---|
|**Basic**|Individual users & small projects|✔ AWS Documentation, ✔ Billing support, ✔ AWS Community Forums|Free|
|**Developer**|Testing & development teams|✔ Email support during business hours, ✔ General guidance|Starts at **$29/month** or **3% of monthly AWS usage**|
|**Business**|Production workloads|✔ 24/7 phone, chat & email support, ✔ AWS Trusted Advisor, ✔ Faster response times|Starts at **$100/month** or **10% of AWS usage**|
|**Enterprise**|Large-scale, mission-critical applications|✔ Dedicated Technical Account Manager (TAM), ✔ Well-Architected Reviews, ✔ 15-minute critical response time|Starts at **$15,000/month** or **10% of AWS usage**|

#### **What is a Technical Account Manager (TAM)?**

A **Technical Account Manager (TAM)** is a **dedicated AWS expert** available in ==**Enterprise Support**== to help businesses **optimize their AWS environments**. TAMs provide **proactive guidance, technical expertise, and strategic planning** to ensure smooth AWS operations.

### **Case severity and response times**

![[Pasted image 20250328172955.png]]


---

# Sample exam question

1- A company wants to centrally manage security policies and billing services within a multi-account AWS environment.  
Which AWS service should the company use to meet these requirements?  
A. AWS Identity and Access Management (IAM)  
==B. AWS Organizations  ==
C. AWS Resource Access Manager (AWS RAM)  
D. AWS Cong  
Correct Answer: B

2- A company wants to have one AWS account for the entire company and individual accounts for each department.  
Which AWS service should the company use to aggregate and manage all accounts?  
A. AWS Billing and Cost Management  
==B. AWS Organizations  ==
C. AWS Identity and Access Management (IAM)  
D. AWS Resource Access Manager  
Correct Answer: B


3- How does the AWS Cloud pricing model differ from the traditional on-premises storage pricing model?  
A. AWS resources do not incur costs  
B. There are no infrastructure operating costs  
==C. There are no upfront cost commitments  ==
D. There are no software licensing costs  
Correct Answer: C

4- AWS has the ability to achieve lower pay-as-you-go pricing by aggregating usage across hundreds of thousands of users.  
This describes which advantage of the AWS Cloud?  
A. Launch globally in minutes  
B. Increase speed and agility  
==C. High economies of scale  ==
D. No guessing about compute capacity  
Correct Answer: C

5- A company runs its workloads on premises. The company wants to forecast the cost of running a large application on AWS.  
Which AWS service or tool can the company use to obtain this information?  
==A. AWS Pricing Calculator  ==
B. AWS Budgets  
C. AWS Trusted Advisor  
D. Cost Explorer  
Correct Answer: A

6- A company wants to eliminate the need to guess infrastructure capacity before deployments. The company also wants to spend its budget on  
cloud resources only as the company uses the resources.  
Which advantage of the AWS Cloud matches the company's requirements?  
A. Reliability  
B. Global reach  
C. Economies of scale  
==D. Pay-as-you-go pricing  ==
Correct Answer: D

7- In which ways does the AWS Cloud offer lower total cost of ownership (TCO) of computing resources than on-premises data centers? (Choose  
two.)  
==A. AWS replaces upfront capital expenditures with pay-as-you-go costs.  ==
B. AWS is designed for high availability, which eliminates user downtime.  
C. AWS eliminates the need for on-premises IT staff.  
==D. AWS uses economies of scale to continually reduce prices.  ==
E. AWS offers a single pricing model for Amazon EC2 instances.  
Correct Answer: AD


8- A company wants to forecast future costs and usage of AWS resources based on past consumption.  
Which AWS service or tool will provide this forecast?  
A. AWS Cost and Usage Report  
B. Amazon Forecast  
C. AWS Pricing Calculator  
==D. Cost Explorer  ==
Correct Answer: D


9-Which of the following are economic advantages of the AWS Cloud? (Choose two.)  
==A. Increased workforce productivity  ==
B. Decreased need to encrypt user data  
C. Manual compliance audits  
D. Simplified total cost of ownership (TCO) accounting  
==E. Faster product launches  ==
Correct Answer: AE

10- A company is planning an infrastructure deployment to the AWS Cloud. Before the deployment, the company wants a cost estimate for running the  
infrastructure.  
Which AWS service or feature can provide this information?  
A. Cost Explorer  
B. AWS Trusted Advisor  
C. AWS Cost and Usage Report  
==D. AWS Pricing Calculator  ==
Correct Answer: D


11- A company needs a quick estimate of the cost to run 1 00 Amazon EC2 instances with AWS Business Support.  
Which tool should the company use to generate the estimate?  
A. AWS Budgets  
B. AWS Cost and Usage Report  
==C. AWS Pricing Calculator  ==
D. Cost Explorer  
Correct Answer: C


12- A company is in the early stages of planning a migration to AWS. The company wants to obtain the monthly predicted total AWS cost of ownership  
for future Amazon EC2 instances and associated storage.  
Which AWS service or tool should the company use to meet these requirements?  
==A. AWS Pricing Calculator  ==
B. AWS Compute Optimizer  
C. AWS Trusted Advisor  
D. AWS Application Migration Service  
Correct Answer: A

13- Which task requires using AWS account root user credentials?  
A. Viewing billing information  
==B. Changing the AWS Support plan  ==
C. Starting and stopping Amazon EC2 instances  
D. Opening an AWS Support case  
Correct Answer: B


14- Which of the following are included in AWS Enterprise Support? (Choose two.)  
==A. AWS technical account manager (TAM)  ==
B. AWS partner-led support  
C. AWS Professional Services  
D. Support of third-party software integration to AWS  
==E. 5-minute response time for critical issues  ==
Correct Answer: AD


15- A company wants to run production workloads on AWS. The company needs concierge service, a designated AWS technical account manager  
(TAM), and technical support that is available 24 hours a day, 7 days a week.  
Which AWS Support plan will meet these requirements?  
A. AWS Basic Support  
==B. AWS Enterprise Support  ==
C. AWS Business Support  
D. AWS Developer Support  
Correct Answer: B




16- Which tasks require use of the AWS account root user? (Choose two.)  
==A. Changing an AWS Support plan  ==
B. Modifying an Amazon EC2 instance type  
C. Grouping resources in AWS Systems Manager  
D. Running applications in Amazon Elastic Kubernetes Service (Amazon EKS)  
==E. Closing an AWS account  ==
Correct Answer: AE


17- A company is migrating to the AWS Cloud. The company requires consultative review and guidance for its applications during the migration. After  
the migration is complete, the company requires a response within 30 minutes if business-critical systems go down.  
Which AWS Support plans meet these requirements? (Choose two.)  
==A. AWS Enterprise Support  
B. AWS Enterprise On-Ramp Support== 
C. AWS Developer Support  
D. AWS Basic Support  
E. AWS Business Support  
Correct Answer: AB

