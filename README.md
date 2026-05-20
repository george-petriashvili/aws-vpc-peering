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

### dev-VPC
![dev-VPC](screenshots/dev-vpc.png)

### prod-VPC
![prod-VPC](screenshots/prod-vpc.png)

### Subnets
![Subnets](screenshots/subnets.png)

### VPC Peering
![Peering](screenshots/peering.png)

### Route Tables (dev)
![RT-dev](screenshots/rt-dev.png)

### Route Tables (prod)
![RT-prod](screenshots/rt-prod.png)

### Security Groups (dev)
![SG-dev](screenshots/sg-dev.png)

### Security Groups (prod)
![SG-prod](screenshots/sg-prod.png)

### Connectivity Test (Ping)
![Ping](screenshots/ping.png)



##  Author
Giorgi Petriashvili
გიორგი პეტრიაშვილი
Giorgi Petriashvili


Network Engineer (NOC Experience)
Building Cloud skills with AWS (VPC, EC2, IAM, S3, CloudWatch)
