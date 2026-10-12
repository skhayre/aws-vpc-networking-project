# AWS VPC Networking Project

## Overview
This project demonstrates how to build a Virtual Private Cloud (VPC) using the AWS Management Console. It covers subnet creation, Availability Zones, internet connectivity and network routing.

## Objectives
- Create a custom AWS VPC.
- Configure two public and two private subnets.
- Distribute subnets across two Availability Zones.
- Create and attach an Internet Gateway.
- Configure a public route table.
- Understand Security Groups and Network ACLs.
- Learn the AWS Shared Responsibility Model.

## Architecture and Configuration

| Component | Configuration |
|---|---|
| AWS Region | Europe (London) - eu-west-2 |
| VPC CIDR | 10.0.0.0/16 |
| Private subnet 1 | 10.0.1.0/24 |
| Private subnet 2 | 10.0.2.0/24 |
| Public subnet 1 | 10.0.3.0/24 |
| Public subnet 2 | 10.0.4.0/24 |
| Availability Zones | eu-west-2a and eu-west-2b |

*Update these values if your actual configuration differs.*

## Implementation
1. Created a VPC with an IPv4 CIDR block.
2. Created two private subnets across separate Availability Zones.
3. Created two public subnets across separate Availability Zones.
4. Configured public IPv4 auto-assignment for public subnets.
5. Created and attached an Internet Gateway.
6. Created a public route table.
7. Added a default route (0.0.0.0/0) targeting the Internet Gateway.
8. Associated the public subnets with the public route table.

## Networking Concepts Learned
- VPCs provide isolated virtual networks.
- CIDR blocks define IP address ranges.
- Subnets divide a VPC into smaller network ranges.
- Availability Zones help improve resilience.
- Internet Gateways and route tables enable internet routing.
- Security Groups are stateful; Network ACLs are stateless.

## AWS Shared Responsibility Model

AWS is responsible for security OF the cloud, including the underlying infrastructure.

The customer is responsible for security IN the cloud, including network access rules, IAM permissions, data protection and workload security.

## Future Improvements
- Launch an EC2 instance in a public subnet.
- Test network connectivity.
- Deploy an EC2 instance in a private subnet.
- Configure and test Security Group and Network ACL rules.
- Explore NAT Gateways for private-subnet outbound internet access.

## Technologies
Amazon VPC, AWS Management Console, IPv4, CIDR, Subnets, Availability Zones, Internet Gateway, Route Tables, Security Groups and Network ACLs.
