# AWS Certified Solutions Architect Associate SAA-C02
By Mark Richman, Ryan Kroonenburg

35 HOURS

159 Lessons 

11 Hands-On Labs 

11 Course Quizzes 

1 Practice Exam

https://acloudguru.com/course/aws-certified-solutions-architect-associate-saa-c02-4KYV

https://www.bilibili.com/video/BV1fV41127vz?p=1

## Chapter 1 Introduction

- An Important Note About A Cloud Guru and Linux Academy Courses 1:18

- Introduction 1:19

- The Exam Blueprint 5:09

- Why Should I Learn and Get Certified with AWS? 13:21

- A Note About Demo Lessons 0:54

## Chapter 2 Supporting Courses

- Certification Path and Supporting Courses 1:15

- Designing Resilient Architectures for Associate AWS Solutions Architects 1:25

- Networking and Compute for Associate AWS Solutions Architects 1:16

- Storage, Databases, and Migration for Associate AWS Solutions Architects 1:18

- High Availability and Scalability for Associate AWS Solutions Architects 1:14

- Application Services for Associate AWS Solutions Architects 1:18

- Logging and Security for Associate AWS Solutions Architects 1:17


## Chapter 3  AWS - 10,000-Foot Overview
- The History of AWS So Far 6:52

- AWS - 10,000-Foot Overview 15:09

- How to Sign up for AWS 3:16

- 10,000 Foot Overview Quiz 15:00 Quiz


## Chapter 4 Identity and Access Management & S3

- Identity and Access Management 101 - 4:34

- Identity and Access Management - Demo 17:35

- Create a Billing Alarm - Demo 4:51

- S3 101 18:39

- Create an S3 Bucket - Demo 11:15

- S3 Pricing Tiers [SAA-C02] 4:38

- S3 Security and Encryption 5:55

- S3 Versioning - Demo 9:13

- Lifecycle Management with S3 - Demo

- S3 Object Lock and Glacier Vault Lock [SAA-C02] 5:08

- S3 Performance [SAA-C02] 6:37

- S3 Select and Glacier Select [SAA-C02] 2:40

- AWS Organizations and Consolidated Billing [SAA-C02] 8:18

- Sharing S3 Buckets Across Accounts - Lab [SAA-C02] 8:32

- Cross-Region Replication - Demo 8:27

- S3 Transfer Acceleration 2:48

- AWS DataSync [SAA-C02] 2:05

- CloudFront 5:08

- Create a CloudFront Distribution - Demo 7:17

- CloudFront Signed URLs and Cookies [SAA-C02] 6:43

- Snowball 4:57

- Snowball - Demo 8:34

- Storage Gateway 10:25

- Athena vs. Macie [SAA-C02] 4:28

- S3 and IAM Summary 17:28

- Creating a Static Website Using Amazon S3 30:00 Hands-On Lab

- Introduction to AWS Identity and Access Management (IAM) - 2020 45:00 Hands-On Lab

- Identity Access Management Quiz

## Chapter 5 EC2
- EC2 101 - Elastic Compute Cloud 14:27

- Launch Our First EC2 Instance: Part 1 - Demo 20:08

- Launch Our First EC2 Instance: Part 2 - Demo 8:36

- Security Groups - Demo 10:02

- EBS 101 3:41

- EBS Volumes and Snapshots - Demo 16:58 

- AMI Types (EBS vs. Instance Store) 7:28  [x]

Amazon Machine Images (AMI)

- ENI vs. ENA vs. EFA [SAA-C02] 6:53

ENI is a virtual network card for EC2


- Encrypted Root Device Volumes and Snapshots - Demo 6:22


- Spot Instances and Spot Fleets [SAA-C02] 8:48


- EC2 Hibernate [SAA-C02] 7:24


- CloudWatch 101 4:47

- CloudWatch - Demo 8:28

- AWS Command Line (CLI) - Demo 7:57

- Identity and Access Management Roles - Demo 5:20 

- Using Bootstrap Scripts - Demo 6:15
EC2启动时执行

```
curl http://169.254.169.254/latest/user-data    # launch script of the EC2
```

- Instance Metadata - Demo 4:17

```
curl http://169.254.169.254/latest/meta-data

curl http://169.254.169.254/latest/user-data    # launch script of the EC2
```

- EFS - Lab [SAA-C02] 12:05
Elastic File System

```
  yum install -y amazon-efs-utils

  mount -t efs -o tls fs-XXXXX:/ /var/www/html
```
Data is stored across multiple AZ's whithin a rergion

Read After Write Consistency


- Amazon FSx for Windows and Amazon FSx for Lustre [SAA-C02] 4:35

- EC2 Placement Groups 6:32
  - Glustered Placement Group:  in single availability zone
  - Spread Placement Group:  on distinct underlying hardware
  - Partitioned Placement Group: 

- HPC on AWS [SAA-C02] 10:42

High Performace Computing


- AWS WAF [SAA-C02] 3:45



- EC2 Summary 18:46

- Using AWS Tags and Resource Groups in AWS 1:00:00 Hands-On Lab

- Creating and Working with an EC2 Instance in AWS 45:00 Hands-On Lab

- Using EC2 Roles and Instance Profiles in AWS 1:30:00 Hands-On Lab

- EC2 Quiz 15:00 Quiz


## Chapter 6 Databases on AWS


Databases 101
11:40
Let's Create Our First RDS Instance - Demo
13:21
RDS: Backups, Multi-AZ, and Read Replicas
7:21
RDS: Backups, Multi-AZ, and Read Replicas - Demo
8:04
DynamoDB
3:52
Advanced DynamoDB [SAA-C02]
13:38
Redshift
6:33
Aurora [SAA-C02]
10:57
Elasticache
3:17
Database Migration Service (DMS) [SAA-C02]
5:26
Caching Strategies on AWS [SAA-C02]
2:58
EMR Overview [SAA-C02]
4:10
Databases Summary
5:52
Deploying an Amazon RDS Multi-AZ and Read Replica in AWS
1:00:00
Hands-On Lab
Databases On AWS Quiz
15:00
Quiz

## Chapter 7 Advanced IAM

AWS Directory Service [SAA-C02]
7:32
IAM Policies [SAA-C02]
15:46
AWS Resource Access Manager (RAM) [SAA-C02]
4:53
AWS Single Sign-On [SAA-C02]
2:57
Advanced IAM Summary [SAA-C02]

## Chapter 8 Route 53


DNS 101
13:56
Register a Domain Name - Demo
7:46
Route 53 Routing Policies Available on AWS
0:39
Route 53: Simple Routing Policy - Demo
3:29
Route 53: Weighted Routing Policy - Demo
7:07
Route 53: Latency-Based Policy - Demo
4:39
Route 53: Failover Routing Policy - Demo
4:03
Route 53: Geolocation Routing Policy - Demo
4:57
Route 53: Geoproximity Routing Policy (Traffic Flow Only) - Demo
3:02
Route 53: Multivalue Answer Policy - Demo
4:03
DNS Summary
5:18
Route 53 Quiz
15:00
Quiz

## Chapter 9 VPCs

VPC Overview
12:11
Create Your Own Custom VPC: Part 1 - Demo
20:27
Create Your Own Custom VPC: Part 2 - Demo
6:39
NAT Instances and NAT Gateways - Demo
13:01
Network Access Control Lists vs. Security Groups - Demo
15:12
Custom VPCs and ELBs - Demo
2:19
VPC Flow Logs - Demo
5:45
Bastions
3:28
Direct Connect
3:39
Setting Up Direct Connect [SAA-C02]
2:37
Global Accelerator [SAA-C02]
11:47
VPC Endpoints [SAA-C02]
10:53
AWS PrivateLink [SAA-C02]
3:36
AWS Transit Gateway [SAA-C02]
2:40
AWS VPN CloudHub [SAA-C02]
2:00
AWS Network Costs [SAA-C02]
3:35
VPC Summary
15:15
Creating a Basic VPC and Associated Components in AWS
45:00
Hands-On Lab
Working with AWS VPC Flow Logs for Network Monitoring - 2020
1:30:00
Hands-On Lab
VPCs Quiz
15:00
Quiz

## Chapter 10 HA Archietcure

Elastic Load Balancers
6:06
Load Balancers and Health Checks - Demo
15:43
Advanced Load Balancer Theory [SAA-C02]
7:03
Auto Scaling [SAA-C02]
5:15
Launch Configurations and Auto Scaling Groups - Demo
8:19
HA Architecture
6:22
Building a Fault-Tolerant WordPress Site: Getting Set Up - Demo
10:31
Building a Fault-Tolerant WordPress Site: Setting Up EC2 - Demo
21:24
Building a Fault-Tolerant WordPress Site: Adding Resilience and Auto Scaling - Demo
20:09
Building a Fault-Tolerant WordPress Site: Cleaning Up - Demo
4:12
Building a Fault-Tolerant WordPress Site: CloudFormation - Demo
6:35
Elastic Beanstalk
5:20
High Availability with Bastion Hosts [SAA-C02]
4:19
On-Premises Strategies with AWS [SAA-C02]
4:37
HA Architecture Summary
7:57
Getting Started with CloudFormation
1:00:00
Hands-On Lab
HA Architecture Quiz

## Chapter 11 Application


SQS [SAA-C02]
10:50
Simple Workflow Service
5:47
Simple Notification Service
4:05
Elastic Transcoder
2:35
API Gateway
9:43
Kinesis 101 [SAA-C02]
9:08
Web Identity Federation and Cognito
7:23
Event Processing Patterns [SAA-C02]
8:13
Applications Summary
8:38
Scaling EC2 Using SQS
45:00
Hands-On Lab
Applications Quiz
15:00
Quiz


## Chapter 12 Security
Reducing Security Threats [SAA-C02]
5:35
Key Management Service (KMS) [SAA-C02]
13:35
CloudHSM [SAA-C02]
3:49
Systems Manager Parameter Store [SAA-C02]
13:08
Secrets Manager [SAA-C02]
2:18
AWS Shield [SAA-C02]
3:15
Web Application Firewall (WAF) [SAA-C02]

## Chapter 13 Serverless

Lambda
13:31
Programmatically Utilizing Data From S3
1:00:00
Hands-On Lab
Let's Build an Alexa Skill - Demo
16:57
Serverless Application Model (SAM) [SAA-C02]
9:23
Elastic Container Service (ECS) [SAA-C02]
18:09
Serverless Summary
3:45
Serverless Quiz
15:00
Quiz

## Chapter 14 6 Lessons Good Luck!

Good Luck and How to Book Your Exam
3:29
Thank You and Next Steps
1:26
Keep Up to Date with AWS This Week
1:02
Challenge Quiz 1
1:15:00
Quiz
Challenge Quiz 2
1:15:00
Quiz
AWS Certified Solutions Architect – Associate Exam
2:15:00
Quiz
