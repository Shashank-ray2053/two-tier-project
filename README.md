                                                                                                                                      # aws-infrastructure-automation-terraform
                                                                                                                                  AWS infrastructure automation using Terraform (IaC)
This repository contains a Terraform project that automates the creation of AWS infrastructure using Infrastructure as Code (IaC).
The main purpose of this project is to practice and demonstrate how AWS resources can be provisioned in a clean, repeatable, and scalable way.

    What this project does
    
Uses Terraform to provision AWS infrastructure

Keeps the configuration modular and reusable

Follows basic security and IaC best practices

Designed for learning as well as real-world reference

This project can be used by anyone who is starting with Terraform on AWS or wants a simple automation example.

Tools and Technologies

Terraform

AWS

Infrastructure as Code (IaC)

AWS Services Used

Depending on the configuration, this project may include:

Amazon EC2

Amazon VPC

Security Groups

Application Load Balancer (ALB)

IAM resources

Project Structure
.
├── main.tf          # Main infrastructure resources
├── provider.tf      # AWS provider configuration
├── variables.tf     # Input variables
├── output.tf        # Output values
├── module/          # Reusable Terraform modules
├── .gitignore       # Terraform and sensitive files
└── README.md

How to run this project
Prerequisites

Terraform installed

AWS CLI installed

AWS credentials configured locally

aws configure

Steps

Clone the repository

git clone https://github.com/Shashank-ray2053/aws-infrastructure-automation-terraform.git


Go to the project directory

cd aws-infrastructure-automation-terraform

Initialize Terraform

terraform init


Review the plan

terraform plan


Apply the configuration

terraform apply

Security notes

Terraform state files are excluded using .gitignore

AWS credentials are not stored in the repository

Variables are used instead of hardcoding values

    What I learned from this project

How Terraform manages AWS resources

How to structure Terraform files properly

How to automate infrastructure using IaC

Importance of security and clean repository setup

Future improvements

Add more AWS services

Improve modularization

Add architecture diagram

Integrate Ansible for configuration management



      License

This project is licensed under the MIT License.
