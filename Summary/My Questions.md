## Read after write consitency

- EFS

- S3
从 2006年第一个云服务对象存储服务 Amazon S3 发布直到 2020年12月1日之前，S3 对象操作都是遵循 eventual consistency 原则
https://aws.amazon.com/blogs/aws/amazon-s3-update-strong-read-after-write-consistency/

到這次更新之前，只有新增的 object 會保證馬上出現。現在則是 update 也會