A NAT gateway forwards traffic from the instances in the private subnet to the internet or other AWS
services, and then sends the response back to the instances. 

The instances in the private subnet cannot be directly accessible from the internet.

After a NAT gateway is created, the route tables for private subnets must be updated to point internet traffic to the NAT gateway.

- Configure a NAT gateway in a public subnet.
- Define a custom route table with a route to the NAT gateway for internet traffic and associate it with the
private subnets for the application tier.
