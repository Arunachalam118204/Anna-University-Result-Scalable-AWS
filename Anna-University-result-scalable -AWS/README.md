# Anna University Result Scalable AWS Architecture

## Overview
Every Anna University student knows the frustration on result day — the website crashes because thousands of students try to access it at the same time.

This project demonstrates a scalable AWS cloud architecture designed to handle heavy traffic during result announcements. The goal is to prevent server crashes and ensure smooth access for all students.

This project focuses purely on cloud infrastructure design using AWS services.

---

## AWS Services Used
- Amazon S3
- AWS Lambda
- Amazon SNS
- Amazon EC2
- Application Load Balancer
- Auto Scaling Group
- Amazon RDS
- Amazon VPC
- IAM

---

## Architecture Workflow
1. Admin uploads the result PDF to **Amazon S3**
2. **AWS Lambda** triggers automatically when the file is uploaded
3. **Amazon SNS** sends email notifications to students
4. Students access the result portal
5. **Application Load Balancer** distributes traffic across EC2 instances
6. **Auto Scaling Group** launches additional instances during heavy traffic
7. **Amazon RDS** runs securely inside a private subnet

---

## Screenshots

### S3 – Result Storage
![S3 Creation](Screenshots/s3-creation.png)
![S3 Upload](Screenshots/s3-upload.png)
![S3 Uploaded](Screenshots/s3-uploaded.png)

### Lambda – Event Trigger
![Lambda Creation](Screenshots/lambda-creation.png)
![Lambda Function View](Screenshots/lambda-functionview.png)
![Lambda Trigger and Code](Screenshots/lambda-triggerandcode.png)

### SNS – Email Notification
![SNS Creation](Screenshots/sns-creation.png)
![SNS Subscription](Screenshots/sns-subcription.png)
![SNS Configuration](Screenshots/sns-configuration.png)

### VPC Network
![VPC](Screenshots/vpc.png)
![Subnets](Screenshots/subnets.png)

### EC2 Deployment
![EC2 Creation](Screenshots/ec2-creation.png)
![EC2 Configuration](Screenshots/ec2-configuration.png)

### Load Balancer
![ELB Creation](Screenshots/elb-creation.png)
![ELB Configuration](Screenshots/elb-configuration.png)
![ELB VPC and Subnets](Screenshots/elb-vpcandsubnets.png)

### Auto Scaling Group
![ASG Creation](Screenshots/asg-creation.png)
![ASG Configuration](Screenshots/asg-configuration.png)
![ASG Instance Management](Screenshots/asg-instancemanagement.png)
![ASG Activity History](Screenshots/asg-activehistory.png)

### RDS Database
![RDS Creation](Screenshots/rds-creation.png)
![RDS Configuration](Screenshots/rds-configuration.png)
![RDS Subnet Group](Screenshots/rds-subnetsgroup.png)

### Email Notification
![Triggered Email](Screenshots/triggered-email.png)
![Email Details](Screenshots/triggered-email-details.png)

### IAM Roles
![IAM Roles](Screenshots/iam-roles.png)
![IAM EC2 Role](Screenshots/iam-ec2role.png)
![IAM Lambda Role](Screenshots/iam-lambdarole.png)

---

## Learning Outcome
- Designed scalable AWS architecture
- Implemented load balancing and auto scaling
- Built event-driven workflow using Lambda and SNS
- Practiced secure VPC networking
- Learned how to handle high traffic systems in cloud

---

## Author
Arunachalam M  
Cloud & Backend Enthusiast  
Preparing for AWS Solutions Architect Associate  

GitHub: https://github.com/Arunachalam118204  
LinkedIn: https://www.linkedin.com/in/arunachalam-murugan-0419192a2