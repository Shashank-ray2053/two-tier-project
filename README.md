Two-Tier Architecture on AWS using Terraform

This project demonstrates a basic two-tier architecture on AWS, built and managed using Terraform. It is designed to help beginners understand how infrastructure can be created and managed as code, while also learning how an application layer and a database layer work together in the cloud.

The setup focuses on simplicity and clarity, making it suitable for learning, practice, and small proof-of-concept projects

Architecture Overview

In this architecture, users access the application through the internet. The application runs on an Amazon EC2 instance deployed in a public subnet. This EC2 instance handles the application logic and communicates with an Amazon RDS database placed in a private subnet. The database is not exposed to the internet, which helps keep the data secure.
All AWS resources in this project are provisioned using Terraform, allowing the infrastructure to be created, updated, and destroyed in a repeatable and reliable way.

Components Created with Terraform

* Amazon VPC
* Public Subnet
* Private Subnet
* Internet Gateway
* Route Tables
* Amazon EC2 (Application Layer)
* Amazon RDS (Database Layer)
* Security Group

How It Works

1. Terraform creates the networking resources (VPC, subnets, route tables).
2. An EC2 instance is launched in the public subnet.
3. An RDS database is created in the private subnet.
4. Security groups control traffic between the EC2 instance and the database.
5. Users access the application through the EC2 instance, which interacts with the database.

Prerequisites

. Basic knowledge of AWS services such as EC2, RDS, and VPC
. Beginner-level understanding of Terraform and Infrastructure as Code
. Terraform installed on your local machine
. AWS CLI configured with valid credentials
. An active AWS account

Basic Networking Knowledge (Helpful)

. What an IP address is
. Difference between public and private IP addresses
. Basic understanding of VPC, subnets, and CIDR blocks
. Familiarity with security groups and how they control traffic

You don’t need deep networking expertise just enough to understand how resources communicate with each other.

How to Deploy

terraform init
terraform plan
terraform apply

How to Destroy the Infrastructure

terraform destroy

Use Cases

1. Learning Terraform basics
2. Understanding two-tier architecture
3. Practicing Infrastructure as Code (IaC)
4. Small demos and proof-of-concept projects

Limitations

* Single Availability Zone
* No load balancer or auto scaling
* Not intended for production use

Note: This project is for learning purposes. Production environments require additional components such as multi-AZ setups, load balancers, NAT gateways, and monitoring.