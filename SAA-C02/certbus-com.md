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
