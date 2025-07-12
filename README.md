# Scalable Web Application with ALB and Auto Scaling

## 1. Project Overview

This project deploys a scalable and highly available web application on AWS using EC2, ALB, and Auto Scaling. It automatically scales based on demand, ensures high availability, and integrates with CloudWatch for continuous monitoring and alerting. Optionally, an RDS database is used for backend storage.
It demonstrates best practices for compute scalability, security, and cost optimization.

## 2. Solution Architecture

## 3. Key AWS Services Used

- Amazon VPC: Creates a logically isolated section of the AWS Cloud where you can launch AWS resources in a virtual network.

- Subnets: Logical subdivisions of a VPC, allowing for organization and isolation of resources.

- Route Tables: Control the flow of network traffic within and out of subnets.

- Internet Gateway (IGW): Enables communication between your VPC and the internet.

- NAT Gateway (NAT GW): Allows instances in private subnets to connect to the internet or other AWS services, while preventing the internet from initiating connections to those instances.

- Security Groups (SG): Act as virtual firewalls to control inbound and outbound traffic for instances and other resources.

- Amazon EC2: Provides resizable compute capacity for hosting the web application.

- Application Load Balancer (ALB): Distributes incoming application traffic across multiple EC2 instances for high availability.

- Auto Scaling Group (ASG): Automatically adjusts the number of EC2 instances based on demand, ensuring availability and optimizing costs.

- Amazon RDS: Managed relational database service (e.g., MySQL/PostgreSQL) with Multi-AZ for high availability.

- IAM: Securely controls access to AWS services and resources, using roles for EC2 instances.

- Amazon CloudWatch & SNS: CloudWatch monitors resources and sets alarms; SNS sends notifications for alerts.

- AWS Systems Manager (SSM) Session Manager: Provides secure, auditable access to EC2 instances without opening inbound ports.