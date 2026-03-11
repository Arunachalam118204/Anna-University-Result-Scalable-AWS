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
File: `s3-creation.png`
![S3 Creation](screenshots/s3-creation.png)

File: `s3-upload.png`
![S3 Upload](screenshots/s3-upload.png)

File: `s3-uploaded.png`
![S3 Uploaded](screenshots/s3-uploaded.png)

---

### Lambda – Event Trigger
File: `lambda-creation.png`
![Lambda Creation](screenshots/lambda-creation.png)

File: `lambda-functionview.png`
![Lambda Function](screenshots/lambda-functionview.png)

File: `lambda-triggerandcode.png`
![Lambda Trigger](screenshots/lambda-triggerandcode.png)

---

### SNS – Email Notification
File: `sns-creation.png`
![SNS Creation](screenshots/sns-creation.png)

File: `sns-subcription.png`
![SNS Subscription](screenshots/sns-subcription.png)

File: `sns-configuration.png`
![SNS Configuration](screenshots/sns-configuration.png)

---

### VPC Network
File: `vpc.png`
![VPC](screenshots/vpc.png)

File: `subnets.png`
![Subnets](screenshots/subnets.png)

---

### EC2 Deployment
File: `ec2-creation.png`
![EC2 Creation](screenshots/ec2-creation.png)

File: `ec2-configuration.png`
![EC2 Config](screenshots/ec2-configuration.png)

---

### Load Balancer
File: `elb-creation.png`
![ELB Creation](screenshots/elb-creation.png)

File: `elb-configuration.png`
![ELB Config](screenshots/elb-configuration.png)

File: `elb-vpcandsubnets.png`
![ELB VPC](screenshots/elb-vpcandsubnets.png)

---

### Auto Scaling Group
File: `asg-creation.png`
![ASG Creation](screenshots/asg-creation.png)

File: `asg-configuration.png`
![ASG Config](screenshots/asg-configuration.png)

File: `asg-instancemanagement.png`
![ASG Instance](screenshots/asg-instancemanagement.png)

File: `asg-activehistory.png`
![ASG Activity](screenshots/asg-activehistory.png)

---

### RDS Database
File: `rds-creation.png`
![RDS Creation](screenshots/rds-creation.png)

File: `rds-configuration.png`
![RDS Config](screenshots/rds-configuration.png)

File: `rds-subnetsgroup.png`
![RDS Subnet](screenshots/rds-subnetsgroup.png)

---

### Email Notification
File: `triggered-email.png`
![Triggered Email](screenshots/triggered-email.png)

File: `triggered-email-details.png`
![Email Details](screenshots/triggered-email-details.png)

---

### IAM Roles
File: `iam-roles.png`
![IAM Roles](screenshots/iam-roles.png)

File: `iam-ec2role.png`
![IAM Role for EC2](screenshots/iam-ec2role.png)

File: `iam-lambdarole.png`
![IAM Role for Lambda](screenshots/iam-lambdarole.png)

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