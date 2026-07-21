---
title: "Week 4"
date: 2026-05-11
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

**Timeline:** 11/5 → 17/5 (5 working days)

## Day 1 - 11/5: Launching an Amazon EC2 Instance

**Tasks Completed:** I began setting up the infrastructure for the project by learning how to launch an Amazon EC2 instance. Using the AWS Management Console, I created an EC2 instance by selecting an appropriate Amazon Machine Image (AMI), choosing a suitable instance type, configuring the Security Group, and generating a Key Pair for secure SSH access from my local computer.

**Knowledge Gained:** I learned that Amazon EC2 is a cloud computing service that provides scalable virtual servers for deploying applications. I also gained a clear understanding of the roles of AMIs, instance types, Key Pairs, and Security Groups during the server provisioning process.

**Achievements:** I successfully launched an EC2 instance, configured the required network ports, and connected to the server via SSH in preparation for application deployment.

**Challenges and Lessons Learned:** I initially encountered an SSH connection error caused by incorrect permissions on the Key Pair file. After correcting the file permissions and verifying the Security Group configuration, I was able to connect successfully. This experience emphasized the importance of reviewing security configurations before deployment.

## Day 2 - 12/5: Configuring Amazon VPC

**Tasks Completed:** After launching the EC2 instance, I studied Amazon Virtual Private Cloud (Amazon VPC). I created a new VPC, configured subnets, attached an Internet Gateway, and updated the Route Table to establish a secure and isolated networking environment for the project.

**Knowledge Gained:** I learned that Amazon VPC provides a private virtual network that allows users to control IP addressing, routing, and network connectivity for AWS resources. I also understood the relationships among VPCs, subnets, Internet Gateways, and Route Tables in designing secure cloud networks.

**Achievements:** I successfully configured a VPC and enabled Internet connectivity for the EC2 instance through an Internet Gateway, allowing the server to access required AWS services.

**Challenges and Lessons Learned:** At first, I confused public and private subnets, which prevented the EC2 instance from accessing the Internet. After reviewing the Route Table and Internet Gateway configuration, I resolved the issue and gained a better understanding of AWS networking.

## Day 3 - 13/5: Working with Amazon DynamoDB

**Tasks Completed:** I studied Amazon DynamoDB and created a database table for the internship project. I selected an appropriate partition key for incident management data and performed CRUD (Create, Read, Update, Delete) operations to evaluate the database's storage and retrieval capabilities.

**Knowledge Gained:** I learned that Amazon DynamoDB is a fully managed NoSQL database service that provides automatic scaling, high performance, and low-latency data access. I also recognized the importance of selecting an appropriate partition key to optimize database performance.

**Achievements:** I successfully created a DynamoDB table and completed CRUD operations, including inserting, updating, deleting, and querying records.

**Challenges and Lessons Learned:** Initially, I did not fully understand how DynamoDB organizes data using partition keys, resulting in an inefficient table design. After studying the AWS documentation, I redesigned the table structure to better suit the project's requirements.

## Day 4 - 14/5: Amazon Cognito and User Authentication

**Tasks Completed:** I studied Amazon Cognito to implement user authentication for the project. I created a User Pool, configured password policies, created test user accounts, and explored the authentication flow used for user login and identity management.

**Knowledge Gained:** I learned that Amazon Cognito is AWS's user authentication and identity management service, supporting user registration, sign-in, and account management. I also understood the role of User Pools in storing user information and handling authentication.

**Achievements:** I successfully created an Amazon Cognito User Pool and verified the authentication process by signing in with a test account.

**Challenges and Lessons Learned:** Configuring the authentication flow involved several options and settings, requiring me to carefully study each mechanism before selecting the most appropriate configuration.

## Day 5 - 15/5: Learning JWT Tokens and Weekly Review

**Tasks Completed:** I continued studying JSON Web Tokens (JWT), which Amazon Cognito uses for user authentication and authorization. I examined the structure of Access Tokens, ID Tokens, and Refresh Tokens and analyzed how these tokens are generated and used after successful user authentication. At the end of the day, I reviewed everything I had learned throughout the week and prepared for integrating AWS services into the project during the following week.

**Knowledge Gained:** I learned that a JWT consists of three parts: the Header, Payload, and Signature. I also understood how Amazon Cognito issues tokens after successful authentication and how these tokens are used to authorize access to protected APIs.

**Achievements:** I gained a solid understanding of authentication using Amazon Cognito and JWT. In addition, I understood how Amazon EC2, Amazon VPC, Amazon DynamoDB, and Amazon Cognito work together within the project's cloud architecture.

**Challenges and Lessons Learned:** This week introduced several new AWS services, making the learning workload quite intensive. I found that drawing architecture diagrams and documenting the relationships between AWS services greatly improved my understanding and made the learning process more effective.
