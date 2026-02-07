# Terraform Private EC2 with ALB and Strapi

## Overview
This project provisions a private EC2 instance inside a VPC using Terraform.  
The instance runs a Strapi application inside Docker.  
An Application Load Balancer (ALB) in the public subnet provides access to the app.

## Architecture
- VPC with public and private subnets
- Internet Gateway for public access
- NAT Gateway for private subnet outbound access
- Private EC2 instance running Strapi
- ALB in public subnets forwarding traffic to EC2

## Prerequisites
- Terraform installed
- AWS CLI configured
- Existing AWS key pair

## Usage

```bash
terraform init
terraform plan
terraform apply
