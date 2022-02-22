## Read after write consistency

- EFS

- S3
从 2006年第一个云服务对象存储服务 Amazon S3 发布直到 2020年12月1日之前，S3 对象操作都是遵循 eventual consistency 原则
https://aws.amazon.com/blogs/aws/amazon-s3-update-strong-read-after-write-consistency/

到這次更新之前，只有新增的 object 會保證馬上出現。現在則是 update 也會





- CloudFront orign access inditiy (OAI)

- Service control policy (SCP) 

- ENI vs EIP

- Read capacity units for strongly consistent reads

- No Upfront (most expensive)

- bastion host

- Security Group source /32 /0

- Perfect Forward Secrecy (PFS) : ELB, CloudFront


- Cloudwatch events
  - Evetn
  - Metrics
  - Alrams

- ASWAuthenticationPlugin




有些答案好像可行，但不是最优解
注意: without requriting changes to the application
cost-efficient architecture

有些题目会考services之间的协同工作，比如 DynamoDB把老数据export到S3
cloudwatch alarm to trigger auto scale
S3 trigger Lambda function




