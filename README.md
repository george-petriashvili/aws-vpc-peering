# aws-vpc-peering

## VPC peering dev-VPC და prod-VPC შორის. უკავშირდება EC2 instance-ს private მისამართზე

## VPC peering between two VPCs to enable private communication between EC2 instances


## Architecture
- dev-VPC (10.0.0.0/16)
	- public-subnet-dev-VPC	10.0.1.0/24
	- private-subnet-dev-VPC  10.0.2.0/24
	- securit group - allows SSH & ICMP
- prod-VPC (10.1.0.0/16)
	- public-subnet-prod-VPC 10.1.1.0/24
	- private-subnet-prod-VPC 10.1.2.0/2
	- securit group - allows SSH & ICMP


## Components
- Public and private subnets
- Internet Gateway
- Route Tables
- Security Groups
- VPC Peering Connection

## Connectivity Test
ტესტირება გავუკეთე WSL-დან, ping გავიდა EC2 instance private IP-ზე
verified connectivity using private IP ping between EC2 instances.


## Screenshots

### VPC Dashboard
![VPC Dashboard](screenshots/vpc-dashboard.png)

### dev-VPC Configuration
![dev-VPC](screenshots/dev-vpc.png)

### prod-VPC Configuration
![prod-VPC](screenshots/prod-vpc.png)

### Public and Private Subnets
![Subnets](screenshots/subnets.png)

### VPC Peering Connection
![VPC Peering](screenshots/peering-active.png)

### Route Tables
![Route Tables](screenshots/route-tables.png)

### Security Groups
![Security Groups](screenshots/security-groups.png)

### Route Table Associations
![Associations](screenshots/subnet-associations.png)

### Successful Ping Test
![Successful Ping](screenshots/successful-ping.png)


##  Author
Giorgi Petriashvili
გიორგი პეტრიაშვილი
Giorgi Petriashvili


Network Engineer (NOC Experience)
Building Cloud skills with AWS (VPC, EC2, IAM, S3, CloudWatch)
