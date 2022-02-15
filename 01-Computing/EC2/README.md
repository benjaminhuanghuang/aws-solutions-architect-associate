# EC2


- EC2 Spot Instances:

Spot Instances would be the least costly option, NOT suitable for jobs that cannot be
interrupted or must complete within a certain time period. Suitable  for the job is stateless in nature, can be started and stopped at any given time with no negative impact

- On-Demand Instances
  Suitable  for the job started and stopped at any given time.
   
  Would be billed for the number of seconds they are running. 



##  Keep the data in instance memory (RAM)
Hibernating an instance saves the contents of RAM to the Amazon EBS root volume. When the instance
restarts, the RAM contents are reloaded.
