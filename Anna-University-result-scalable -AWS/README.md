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
![S3 Creation](screenshots/S3-creation.png)
![S3 Upload](screenshots/S3-upload.png)
![S3 Uploaded](screenshots/S3-uploaded.png)

### Lambda – Event Trigger
![Lambda Creation](screenshots/LAMBDA-creation.png)
![Lambda Function](screenshots/LAMBDA-FunctionVIEW.png)
![Lambda Trigger](screenshots/LAMBDA-Trigger-code.png)

### SNS – Email Notification
![SNS Creation](screenshots/SNS-creation.png)
![SNS Subscription](screenshots/SNS-subcription.png)
![SNS Configuration](screenshots/SNS-configuration.png)

### VPC Network
![VPC](screenshots/VPC.png)
![Subnets](screenshots/SUBNETS.png)

### EC2 Deployment
![EC2 Creation](screenshots/EC2-creation.png)
![EC2 Config](screenshots/EC2-configuration.png)

### Load Balancer
![ELB Creation](screenshots/ELB-creation.png)
![ELB Config](screenshots/ELB-configuration.png)
![ELB VPC](screenshots/ELB-vpc-subnets.png)

### Auto Scaling Group
![ASG Creation](screenshots/ASG-creation.png)
![ASG Config](screenshots/ASG-configuration.png)
![ASG Instance](screenshots/ASG-instancemanagement.png)
![ASG Activity](screenshots/ASG-activehistory.png)

### RDS Database
![RDS Creation](screenshots/RDS-creation.png)
![RDS Config](screenshots/RDS-configuration.png)
![RDS Subnet](screenshots/RDS-subnetsgroup.png)

### Email Notification
![Triggered Email](screenshots/TRIGGERED_EMAIL.png)
![Email Details](screenshots/TRIGGERED_EMAIL_DETAILS.png)

### IAM Roles
![IAM Roles](screenshots/IAM-Roles.png)
![IAM Role for EC2](screenshots/IAM-ec2-role.png)
![IAM Role for Lambda](screenshots/IAM-lambda-role.png)


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
LinkedIn: www.linkedin.com/in/arunachalam-murugan-0419192a2