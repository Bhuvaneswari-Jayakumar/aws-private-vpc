# AWS Cloud Deployment: Scalable & Secure Python Server Setup

## Project Overview
This project demonstrates the deployment of a simple Python HTTP server in a private subnet within a Virtual Private Cloud (VPC) on Amazon AWS. The deployment leverages AWS features such as Auto Scaling and an Application Load Balancer (ALB) to ensure scalability and secure traffic management.

## Key Features
- **Python HTTP Server**: A basic Python HTTP server is deployed in a private subnet.
- **Scalability**: Configured Auto Scaling to manage server instances based on demand.
- **Traffic Management**: Used an Application Load Balancer (ALB) to route traffic to the server instances.
- **Network Security**: Access managed through a bastion host for secure SSH login.

## Steps to Deploy the Server

### 1. Set Up VPC
- Create a VPC with both public and private subnets.

### 2. Launch EC2 Instances
- Launch an EC2 instance in the private subnet to run the Python HTTP server using `python -m http.server 8080`.

### 3. Configure Auto Scaling
- Set up an Auto Scaling Group to automatically adjust the number of EC2 instances based on traffic demand.

### 4. Set Up Application Load Balancer (ALB)
- Create an ALB to distribute traffic securely to the EC2 instances in the private subnet.

### 5. Configure Network Access
- Use a bastion host in the public subnet to SSH into the EC2 instance in the private subnet.
- Ensure the ALB is configured to route traffic to the server when it is running.

## Accessing the Server
- The server is accessible through the DNS name provided by the ALB: `production-project-vpc-818228988.ap-south-1.elb.amazonaws.com`.
- Access is controlled through the VPC configuration and network security settings.

## Lessons Learned
- Gained a foundational understanding of AWS VPCs, subnets, and network security.
- Enhanced knowledge of AWS Auto Scaling and traffic management using ALB.

## Conclusion git push origin main
git push origin main

This project provided hands-on experience with deploying and managing a Python server in a cloud environment, leveraging AWS features for scalability and security.

## Contact Information
For any questions or further discussion, please contact me at [bhuvaneswarijayakumar475@gmail.com](mailto:bhuvaneswarijayakumar475@gmail.com).

## Project Link
[GitHub Repository](https://github.com/Bhuvaneswari-Jayakumar/aws-private-vpc)
