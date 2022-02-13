QUESTION 1
A security learn needs to enforce the rotation of all 1AM users' access keys every 90 days If an access key Is found to
be older, the key must be made inactive and removed. A solutions architect must create a solution that will check for and
remediate any keys older than 90 days

Which solution meets these requirements with the LEAST operational effort?

A. Create an AWS Config rule to check for the key age Configure the AWS Config rule to run an AWS Batch job to
remove the key

B. Create an Amazon EventBridge (Amazon CloudWatch Events) rule to check for the key age Configure the rule to run
an AWS Batch job to remove the key

C. Create an AWS Config rule to check for the key age Define an Amazon EventBridge (Amazon CloudWatch Events)
rule to schedule an AWS Lambda function to remove the key

D. Create an Amazon EventBridge (Amazon CloudWatch Events) rule to check for the key age Define an EventBridge
(CloudWatch Events) rule to run an AWS Batch job to remove the key

Correct Answer: C 


QUESTION 2
An application development team is designing a microservice that will convert large images to smaller compressed
images When a user uploads an image through the web interface the microservice should store the image in an
Amazon S3 bucket process and compress the image with an AWS Lambda function, and store the image in its
compressed form m a different S3 bucket.

A solutions architect needs to design a solution that uses durable stateless components to process the images
automatically.
Which combination of actions will meet these requirements? (Select TWO )

A. Create an Amazon Simple Queue Service (Amazon SQS) queue Configure the S3 bucket to send a
notification to the SQS queue when an image is uploaded to the S3 bucket

B. Configure the Lambda function to use the Amazon Simple Queue Service (Amazon SQS) queue as the invocation
source When the SQS message is successfully processed, delete the message in the queue

C. Configure the Lambda function to monitor the S3 bucket for new uploads When an uploaded image is detected write
the file name to a text file in memory and use the text file to keep track of the images that were processed

D. Launch an Amazon EC2 instance to monitor an Amazon Simple Queue Service (Amazon SQS) queue When items
are added to the queue log the file name in a text file on the EC2 instance and invoke the Lambda function

E. Configure an Amazon EventBridge (Amazon CloudWatch Events) event to monitor the S3 bucket When an image is
uploaded send an alert to an Amazon Simple Notification Service (Amazon SNS) topic with the application owner\\'s
email address for further processing 

Correct Answer: AB 


QUESTION 4
A solutions architect is designing a new workload in which an AWS Lambda function will access an Amazon DynamoDB
table. What is the MOST secure means of granting the Lambda function access tothe DynamoDB labia?

A. Create an IAM role with the necessary permissions to access the DynamoDB table Assign the role to the Lambda
function.

B. Create a DynamoDB user name and password and give them to the developer to use in the Lambda function.

C. Create an IAM user, and create access and secret keys for the user. Give the user the necessary permissions to
access the DynarnoOB table. Have the developer use these keys to access the resources.

D. Create an IAM role allowing access from AWS Lambda Assign the role to the DynamoDB table

Correct Answer: A 


QUESTION 5
A company runs a high performance computing (HPC) workload on AWS. The workload required low-latency network
performance and high network throughput with tightly coupled node-to-node communication. The Amazon EC2
instances are properly sized for compute and storage capacity, and are launched using default options. What should a
solutions architect propose to improve the performance of the workload?
A. Choose a cluster placement group while launching Amazon EC2 instances
B. Choose dedicated instance tenancy while launching Amazon EC2 instances
C. Choose an Elastic Inference accelerator while launching Amazon EC2 instances
D. Choose the required capacity reservation while launching Amazon EC2 instances.

Correct Answer: A


QUESTION 1
A company has an AWS Lambda function that needs read access to an Amazon S3 bucket that is located in the same
AWS account. Which solution will meet these requirement in the MOST secure manner?
A. Apply an S3 bucket pokey that grants road access to the S3 bucket
B. Apply an IAM role to the Lambda function Apply an 1AM policy to the role to grant read access to the S3 bucket
C. Embed an access key and a secret key In the Lambda function\\'s coda to grant the required 1AM permissions for
read access to the S3 bucket
D. Apply an IAM role to the Lambda function. Apply an IAM policy to the role to grant read access to all S3 buckets In
the account

Correct Answer: B 


QUESTION 2
A company has a custom application running on an Amazon EC2 instance that:
1. Reads a large amount of data from Amazon S3
2. Performs a multi-stage analysis.
3. Writes the results to Amazon DynamoDB.

The application writes a significant number of large, temporary files during the multi-stage analysis. The process
performance depends on the temporary storage performance. What would be the fastest storage option for holding the
temporary files?
A. Multiple Amazon S3 buckets with Transfer Acceleration for storage
B. Multiple Amazon EBS drives with Provisioned IOPS and EBS optimization.
C. Multiple Amazon EFS volumes using the Network File System version 4.1 (NFSv4.1) protocol.
D. Multiple instance store volumes with software RAID 0.

Correct Answer: A 

QUESTION 3
A company's web application uses an Amazon RDS PostgreSQL DB instance to store its application data. During the
financial closing period at the start of every month. Accountants run large queries that impact the database's
performance due to high usage. The company wants to minimize the impact that the reporting activity has on the web
application. What should a solutions architect do to reduce the impact on the database with the LEAST amount of
effort?
A. Create a read replica and direct reporting traffic to the replica.
B. Create a Multi-AZ database and direct reporting traffic to the standby.
C. Create a cross-Region read replica and direct reporting traffic to the replica.
D. Create an Amazon Redshift database and direct reporting traffic to the Amazon Redshift database.

Correct Answer: A

Amazon RDS uses the MariaDB, MySQL, Oracle, PostgreSQL, and Microsoft SQL Server DB engines' built-in
replication functionality to create a special type of DB instance called a read replica from a source DB instance. Updates
made to the source DB instance are asynchronously copied to the read replica. You can reduce the load on your source
DB instance by routing read queries from your applications to the read replica. When you create a read replica, you first
specify an existing DB instance as the source. Then Amazon RDS takes a snapshot of the source instance and creates
a read-only instance from the snapshot. Amazon RDS then uses the asynchronous replication method for the DB
engine to update the read replica whenever there is a change to the source DB instance. The read replica operates as a
DB instance that allows only read-only connections. Applications connect to a read replica the same way they do to any
DB instance. Amazon RDS replicates all databases in the source DB instance.
https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_ReadRepl.html 

QUESTION 4
A company is using an Application Load Balancer (ALB) to present its application to the internet. The company finds
abnormal traffic access patterns across the application. A solutions architect needs to improve visibility into the
infrastructure to help the company understand these abnormalities better
What is the MOST operationally efficient solution that meets these requirements?
A. Create a table in Amazon Athena for AWS CloudTrail logs Create a query for the relevant information.
B. Enable ALB access logging to Amazon S3. Create a table in Amazon Athena, and query the logs
C. Enable ALB access logging to Amazon S3 Open each file m a text editor, and search each line for the relevant
information
D. Use Amazon EMR on a dedicated Amazon EC2 instance to directly query the ALB to acquire traffic access log
information
Correct Answer: B
Reference: https://aws.amazon.com/blogs/big-data/catalog-and-analyze-application-load-balancer-logsmore-efficientlywith-aws-glue-custom-classifiers-and-amazon-athena/ 

QUESTION 5
A company wants to use an AWS Region as a disaster recovery location for its on-premises infrastructure. 
The company has 10 TB of existing data, and the on-premise data center has a 1 Gbps internet
connection. A solutions architect must find a solution so the company can have its existing data on AWS in
72 hours without transmitting it using an unencrypted channel.
Which solution should the solutions architect select?
A. Send the initial 10 TB of data to AWS using FTP.
B. Send the initial 10 TB of data to AWS using AWS Snowball.
C. Establish a VPN connection between Amazon VPC and the company's data center.
D. Establish an AWS Direct Connect connection between Amazon VPC and the company's data center.
Correct Answer: C 


QUESTION 1
A company has an internet-facing application that runs on premises. The application contains mostly user-generated
content. The data is stored in an on-premises network- attached storage system. The company wants to archive this
data annually and has chosen to move the archival data to Amazon S3. The company needs a solution to migrate the
archival data into an S3 bucket.
Which solution will meet these requirements?

A. Use AWS Storage Gateway Volume Gateway. Cache the data, and then replicate the data from the on-premises
environment to Amazon S3.
B. Use AWS DataSync. Create a configuration to replicate the data from the on-premises environment to Amazon S3.
C. Use AWS Transfer Family. Use an SFTP client to serially transfer the data from the on- premises environment to
Amazon S3.
D. Use Amazon S3 Transfer Acceleration. Use a third-party backup utility to replicate the data from the on-premises
environment to Amazon S3.

Correct Answer: B 

QUESTION 2
A city has deployed a web application running on AmazonEC2 instances behind an Application Load Balancer (ALB)
The Application's users have reported sporadic performance, which appears to be related to DDoS attacks originating
from random IP addresses. The City needs a solution that requires minimal configuration changes and provides an audit
trail for the DDoS source. Which solution meets these requirements..?
A. Enable an AWS WAF web ACL on the ALB and configure rules to block traffic from unknown sources.
B. Subscribe to Amazon inspector. Engage the AWS DDoS Resource Team (DRT) to integrate migrating controls into
the service.
C. Subscribe to AWS shield advanced. Engage the AWS DDoS Response team (DRT) to integrate migrating controls
into the service.
D. Create an Amazon CloudFront distribution for the application and set the ALB as the origin. Enable an AWS WAF
web ACL on the distribution and configure rules to block traffic from unknown sources.

Correct Answer: C

QUESTION 3
A company's website handles millions of requests each day. and the number of requests continues to increase. A
solutions architect needs to improve the response time of the web application. The solutions architect determines that
the application needs to decrease latency when retrieving product details from the Amazon DynamoDB table
A. Set up a DynamoOB Accelerator (DAX) cluster Route all read requests through DAX.
B. Set up Amazon ElasliCache (or Redis between the DynamoOB table and the web application.Route all read requests
through Redis.
C. Set up Amazon ElasliCache for Memcached between the DynamoOB table and the web application Route all read
requests through Memcached.
D. Set up Amazon DynamoOB Streams on the table, and have AWS Lambda read from the table and populate Amazon
ElastiCache. Route all read requests through ElasliCache

Correct Answer: A 

QUESTION 4
A company has an automobile sales website that stores its listings in an database on Amazon RDS When an
automobile is sold, the listing needs to be removed from the website and the data must be sent to multiple target
systems.
Which design should a solutions architect recommend?
A. Create an AWS Lambda function triggered when the database on Amazon RDS is updated to send the information to
an Amazon Simple Queue Service (Amazon SQS) queue for the targets to consume.
B. Create an AWS Lambda function triggered when the database on Amazon RDS is updated to send the information to
an Amazon Simple Queue Service (Amazon SQS) FIFO queue for the targets to consume
C. Subscribe to an RDS event notification and send an Amazon Simple Queue Service (Amazon SQS) queue fanned
out to multiple Amazon Simple Notification Service (Amazon SNS) topics Use AWS Lambda functions to update the
targets
D. Subscribe to an RDS event notification and send an Amazon Simple Notification Service (Amazon SNS) topic fanned
out to multiple Amazon Simple Queue Service (Amazon SQS) queues Use AWS Lambda functions to update the
targets
Correct Answer: D


QUESTION 5
Which solution should the company use for the data transfer to meet these requirements?
A. AWS DataSync
B. AWS Migration Hub
C. AWS Snowball Edge Storage Optimized
D. AWS Transfer for SFTP
Correct Answer: A 


QUESTION 1
A company wants to build a scalable key management infrastructure to support developers who need to encrypt data in
their applications. What should a solutions architect do to reduce the operational burden?

A. Use multi-factor authentication (MFA) to protect the encryption keys
B. Use AWS Key Management Service (AWS KMS) to protect the encryption keys
C. Use AWS Certificate Manager (ACM) to create, store and assign the encryption keys
D. Use an IAM policy to limit the scope of users who have access permissions to protect the encryption keys
Correct Answer: B


QUESTION 2
A company runs a public three-Tier web application in a VPC The application runs on Amazon EC2 instances across
multiple Availability Zones. The EC2 instances that run in private subnets need to communicate with a license server
over the internet The company needs a managed solution that minimizes operational maintenance
Which solution meets these requirements?

A. Provision a NAT instance in a public subnet Modify each private subnets route table with a default route that points to
the NAT instance
B. Provision a NAT instance in a private subnet Modify each private subnet's route table with a default route that points
to the NAT instance
C. Provision a NAT gateway in a public subnet Modify each private subnet's route table with a default route that points
to the NAT gateway
D. Provision a NAT gateway in a private subnet Modify each private subnet's route table with a default route that points
to the NAT gateway .

Correct Answer: C 

QUESTION 3
A company has a highly dynamic batch processing job that uses many Amazon EC2 instances to complete it. The job is
stateless in nature, can be started and stopped at any given time with no negative impact, and typically takes upwards
of 60 minutes total to complete The company has asked a solutions architect to design a scalable and cost-effective
solution that meets the requirements of the job.
What should the solutions architect recommend?
A. Implement EC2 Spot Instances
B. Purchase EC2 Reserved Instances
C. Implement EC2 On-Demand Instances 
D. Implement the processing on AWS Lambda

Correct Answer: A

QUESTION 4
A company's application is running on Amazon EC2 instances m a single Region in the event of a disaster a solutions
architect needs to ensure that the resources can also be deployed to a second Region Which combination of actions
should the solutions architect take to accomplish this? (Select TWO)

A. Detach a volume on an EC2 instance and copy it to Amazon S3
B. Launch a new EC2 instance from an Amazon Machine image (AMI) in a new Region
C. Launch a new EC2 instance in a new Region and copy a volume from Amazon S3 to the new instance
D. Copy an Amazon Machine Image (AMI) of an EC2 instance and specify a different Region for the destination
E. Copy an Amazon Elastic Block Store (Amazon EBS) volume from Amazon S3 and launch an EC2 instance in the
destination Region using that EBS volume

Correct Answer: BD

Cross Region EC2 AMI Copy
We know that you want to build applications that span AWS Regions and we\\'re working to provide you with the
services and features needed to do so. We started out by launching the EBS Snapshot Copy feature late last year. This
feature gave you the ability to copy a snapshot from Region to Region with just a couple of clicks. In addition, last month
we made a significant reduction (26% to 83%) in the cost of transferring data between AWS Regions, making it less
expensive to operate in more than one AWS region. Today we are introducing a new feature: Amazon Machine Image
(AMI) Copy. AMI Copy enables you to easily copy your Amazon Machine Images between AWS Regions. AMI Copy
helps enable several key scenarios including: Simple and Consistent Multi-Region Deployment ?You can copy an AMI
from one region to another, enabling you to easily launch consistent instances based on the same AMI into different
regions. Scalability You can more easily design and build world-scale applications that meet the needs of your users,
regardless of their location.
Performance You can increase performance by distributing your application and locating critical components of your
application in closer proximity to your users. You can also take advantage of region-specific features such as instance
types or other AWS services. Even Higher Availability You can design and deploy applications across AWS regions, to
increase availability. Once the new AMI is in an Available state the copy is complete.
https://aws.amazon.com/blogs/aws/ec2-ami-copy-between-regions/ 


QUESTION 5
A company has a 143 TB MySQL database that it wants to migrate to AWS. The plan is to use Amazon
Aurora MySQL as the platform going forward. The company has a 100 Mbps AWS Direct Connect
connection to Amazon VPC.
Which solution meets the company's needs and takes the LEAST amount of time? 

A. Use a gateway endpoint for Amazon S3 Migrate the data to Amazon S3 Import the data into Aurora
B. Upgrade the Direct Connect link to 500 Mbps. Copy the data to Amazon S3 Import the data into Aurora
C. Order an AWS Snowmobile and copy the database backup to it. Have AWS import the data into Amazon S3 Import
the backup into Aurora
D. Order four 50-TB AWS Snowball devices and copy the database backup onto them. Have AWS import the data into
Amazon S3 Import the data into Aurora

Correct Answer: D 

QUESTION 1
A city has deployed a web application running on AmazonEC2 instances behind an Application Load Balancer (ALB)
The Application's users have reported sporadic performance, which appears to be related to DDoS attacks originating
from random IP addresses. The City needs a solution that requires minimal configuration changes and provides an audit
trail for the DDoS source. Which solution meets these requirements..?
A. Enable an AWS WAF web ACL on the ALB and configure rules to block traffic from unknown sources.
B. Subscribe to Amazon inspector. Engage the AWS DDoS Resource Team (DRT) to integrate migrating controls into
the service.
C. Subscribe to AWS shield advanced. Engage the AWS DDoS Response team (DRT) to integrate migrating controls
into the service.
D. Create an Amazon CloudFront distribution for the application and set the ALB as the origin. Enable an AWS WAF
web ACL on the distribution and configure rules to block traffic from unknown sources.

Correct Answer: C 

QUESTION 2
A mobile gaming company runs application servers on Amazon EC2 instances. The servers receive updates from
players every 15 minutes. The mobile game creates a JSON object of the progress made in the game since the last
update, and sends the JSON object to an Application Load Balancer. As the mobile game is played, game updates are
being lost. The company wants to create a durable way to get the updates in older. What should a solutions architect
recommend to decouple the system?

A. Use Amazon Kinesis Data Streams to capture the data and store the JSON object in Amazon S3.
B. Use Amazon Kinesis Data Firehose to capture the data and store the JSON object in Amazon S3.
C. Use Amazon Simple Queue Service (Amazon SQS) FIFO queues to capture the data and EC2 instances to process
the messages in the queue.
D. Use Amazon Simple Notification Service (Amazon SNS) to capture the data and EC2 instances to process the
messages sent to the Application Load Balancer.

Correct Answer: C 

QUESTION 3
A company is building its web application using containers on AWS. The company requires three instances of the web
application to run at all times. The application must be able to scale to meet increases in demand. Management is
extremely sensitive to cost but agrees that the application should be highly available.
What should a solutions architect recommend?

A. Create an Amazon Elastic Container Service (Amazon ECS) cluster using the Fargate launch type.Create a task
definition for the web application. Create an ECS service with a desired count of three tasks. 
B. Create an Amazon Elastic Container Service (Amazon ECS) cluster using the Amazon EC2 launch type with three
container instances in one Availability Zone. Create a task definition for the web application. Place one task for each
container instance.
C. Create an Amazon Elastic Container Service (Amazon ECS) cluster using the Fargate launch type with one container
instance in three different Availability Zones. Create a task definition for the web application. Create an ECS service with
a desired count of three tasks.
D. Create an Amazon Elastic Container Service (Amazon ECS) cluster using the Amazon EC2 launch type with one
container instance in two different Availability Zones. Create a task definition for the web application. Place two tasks on
one container instance and one task on the remaining container instance.

Correct Answer: D

QUESTION 4
A web application is deployed in the AWS Cloud It consists of a two-tier architecture that includes a web layer and a
database layer The web server is vulnerable to cross-site scripting (XSS) attacks What should a solutions architect do to
remediate the vulnerability?
A. Create a Classic Load Balancer Put the web layer behind the load balancer and enable AWS WAF
B. Create a Network Load Balancer Put the web layer behind the load balancer and enable AWS WAF
C. Create an Application Load Balancer Put the web layer behind the load balancer and enable AWS WAF
D. Create an Application Load Balancer Put the web layer behind the load balancer and use AWS Shield Standard

Correct Answer: C
WAF = Web Application Firewall
Working with cross-site scripting match conditions Attackers sometimes insert scripts into web requests in an effort to
exploit vulnerabilities in web applications. You can create one or more cross-site scripting match conditions to identify
the parts of web requests, such as the URI or the query string, that you want AWS WAF Classic to inspect for possible
malicious scripts. Later in the process, when you create a web ACL, you specify whether to allow or block requests that
appear to contain malicious scripts. Web Application Firewall
You can now use AWS WAF to protect your web applications on your Application Load Balancers. AWS WAF is a web
application firewall that helps protect your web applications from common web exploits that could affect application
availability, compromise security, or consume excessive resources.
https://docs.aws.amazon.com/waf/latest/developerguide/classic-web-acl-xss-conditions.html
https://aws.amazon.com/elasticloadbalancing/features/

QUESTION 5
A company with a single AWS account runs its internet-facing containerized web application on an Amazon Elastic
Kubernetes Service (Amazon EKS) cluster. The EKS cluster is placed in a private subnet of a VPC. System
administrators access the EKS cluster through a bastion host on a public subnet.
A new corporate security policy requires the company to avoid the use of bastion hosts. The company also must not
allow internet connectivity to the EKS cluster. 
Which solution meets these requirements MOST cost-effectively?

A. Set up an AWS Direct Connect connection.
B. Create a transit gateway.
C. Establish a VPN connection.
D. Use AWS Storage Gateway.

Correct Answer: B 

QUESTION 1
A solutions architect is tasked with transferring 750 TB of data from a network-attached file system located
at a branch office to Amazon S3 Glacier The solution must avoid saturating the branch office's lowbandwidth internet connection.
What is the MOST cost-effective solution?

A. Create a site-to-site VPN tunnel to an Amazon S3 bucket and transfer the files directly Create a bucket policy to
enforce a VPC endpoint
B. Order 10 AWS Snowball appliances and select an S3 Glacier vault as the destination Create a bucket policy to
enforce a VPC endpoint
C. Mount the network-attached file system to Amazon S3 and copy the files directly. Create a lifecycle policy to
transition the S3 objects to Amazon S3 Glacier
D. Order 10 AWS Snowball appliances and select an Amazon S3 bucket as the destination. Create a lifecycle policy to
transition the S3 objects to Amazon S3 Glacier

Correct Answer: D
Regional Limitations for AWS Snowball
The AWS Snowball service has two device types, the standard Snowball and the Snowball Edge. The following table
highlights which of these devices are available in which regions. 

QUESTION 2
A company is running a multi-tier web application on AWS. The application runs its database tier on Amazon Aurora
MySQL. The application and database tiers are in the us-east-1 Region A database administrator who regularly
monitors the Aurora DB cluster finds that an intermittent increase in read traffic is creating high CPU utilization on the
read replica and causing increased read latency of the application What should a solutions architect do to improve read
scalability?
A. Reboot the Aurora DB cluster
B. Create a cross-Region read replica
C. Increase the instance class of the read replica
D. Configure Aurora Auto Scaling for the read replica

Correct Answer: D 

QUESTION 3

A company is using Amazon Redshift for analytics and to generate customer reports. The company recently acquired 50
TB of additional customer demographic data. The .........S3. The company needs a solution that joins the data and
visualizes the results with the least possible cost and effort.
What should a solutions architect recommend to meet these requirements?

A. Use Amazon Redshift Spectrum to query the data in Amazon S3 directly and join that data with the existing data in
Amazon Redshift. Use Amazon QuickSight to....
B. Use Amazon Athena to query the data in Amazon S3. Use Amazon QuickSight to join the data from Athena with the
existing data in Amazon Redshift and to build...
C. Increase the size of the Amazon Redshift cluster, and load the data from Amazon S3. Use Amazon EMR Notebooks
to query the data and build the visualizations,,,
D. Export the data from the Amazon Redshift cluster into Apache Parquet files in Amazon S3. Use Amazon
Elasticsearch Service (Amazon ES) to query the data. Use..

Correct Answer: B 

QUESTION 4
A company wants to run a static website served through Amazon CloudFront. What is an advantage of storing the
website content in an Amazon S3 bucket instead of an Amazon Elastic Block Store (Amazon EBS) volume?

A. S3 buckets are replicated globally, allowing for large scalability. EBS volumes are replicated only within an AWS
Region.
B. S3 is an origin for CloudFront. EBS volumes would need EC2 instances behind an Elastic Load Balancing load
balancer to be an origin
C. S3 buckets can be encrypted, allowing for secure storage of the web files. EBS volumes cannot be encrypted. 
D. S3 buckets support object-level read throttling, preventing abuse. EBS volumes do not provide object-level throttling.

Correct Answer: B
"For static files, store the definitive versions of your files in one or more origin servers. These could be Amazon S3
buckets. For your dynamically generated content that is personalized or customized, you can use Amazon EC2"


QUESTION 5
A solutions architect is designing a highly available website that is served by multiple web servers hosted outside of
AWS. If an instance becomes unresponsive, the architect needs to remove it from the rotation. What is the MOST
efficient way to fulfill this requirement?

A. Use Amazon CloudWatch to monitor utilization.
B. Use Amazon API Gateway to monitor availability.
C. Use an Amazon Elastic Load Balancer.
D. Use Amazon Route 53 health checks.

Correct Answer: C 
