# AWS-Interview-Prep

1) Eplain the Steps to set up a secured VPC with subnets and everything?

a) Create VPC:
Define VPC CIDR block and tenancy 
Enable DNS support and DNS Host names if needed

b) Create subnets:
Allocate CIDR blocks for subnets
Spread Subnets across availability zones for redundancy

c) Configure Ruote tables:
Define routes for internet-bound traffic
Associate subnets with route tables

d)Setup NACLS 
Configure Inbound and outbound rules
Associate NACL's with subnets

e) Implement Security groups

Define Inbound and outbound rules
Associate security groups with instance

f) Add Internetgateway(IGW)
   Attach IGW to VPC
   Update route tables for internet access

g) Optional NATGateway/Instance:
   Setup in Public subnet for private subnet internet access

h) Enable Monitoring:
   Enable VPC Flow logs for traffic analysis
   Monitor with Cloudwatch

2) Load Balancers: These are used to manage the traffic for multiple servers/Instances

a) Application Load balancer : To Manage the traffice related to HTTP and HTTPS will use application load balancer
b) Network Load balancer: To Manage the traffic related to TCP/UDP it will be used
c) Gateway Load balancer: To Manage the traffic related to third party tools it will be used
d) Classic load balancer: whiich is a legacy load balancer

