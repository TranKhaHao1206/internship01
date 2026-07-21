---
title: "Week 5"
date: 2026-05-18
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

**Timeline:** 18/5 → 24/5 (5 working days)

## Day 1 - 18/5: Learning AWS Lambda and the Function as a Service (FaaS) Model

**Tasks Completed:** I began studying AWS Lambda, AWS's serverless computing service. I explored how Lambda functions operate, created my first Lambda function using Node.js, and wrote simple code to process user requests. I also learned how to deploy and test Lambda functions directly through the AWS Management Console.

**Knowledge Gained:** I learned that AWS Lambda allows developers to execute code without managing servers. Developers only need to focus on writing application logic, while AWS automatically provisions resources, scales the infrastructure, and manages server operations whenever the function is invoked.

**Achievements:** I successfully created my first Lambda function and tested it using sample events provided by AWS.

**Challenges and Lessons Learned:** At first, I was unfamiliar with the serverless computing model because there was no need to configure or manage servers as with Amazon EC2. After several hands-on exercises, I gained a better understanding of Lambda's event-driven execution model.

## Day 2 - 19/5: Integrating AWS Lambda with Amazon DynamoDB

**Knowledge Gained:** I learned how the AWS SDK enables Lambda functions to connect to DynamoDB and perform database operations. I also studied the use of IAM Roles to grant Lambda secure access to database resources.

**Knowledge learned:** API Gateway is the entry point of serverless backend services and can handle routing, authentication, CORS, and throttling.

**Achievements:** I successfully enabled Lambda functions to read from and write to DynamoDB, giving me a clearer understanding of data processing within a serverless architecture.

**Challenges and Lessons Learned:** During implementation, the Lambda function encountered permission errors when accessing DynamoDB. After reviewing the IAM Role configuration and attaching the appropriate IAM Policy, I resolved the issue successfully.

## Day 3 - 20/5: Learning Amazon API Gateway and Amazon Cognito

**Tasks Completed:** I studied Amazon API Gateway and its role in building RESTful APIs. I also explored how Amazon API Gateway integrates with Amazon Cognito to authenticate users before allowing access to protected APIs.

**Knowledge Gained:** I learned that Amazon API Gateway serves as the entry point for client requests, forwarding them to AWS Lambda for processing and returning responses to users. Amazon Cognito handles user authentication and issues JWT tokens to secure API access.

**Achievements:** I gained a clear understanding of the request flow from the client to API Gateway, Lambda, DynamoDB, and back to the client. I also understood how Amazon Cognito participates in the authentication process.

**Challenges and Lessons Learned:** Initially, I found it difficult to understand how API Gateway, Lambda, and Cognito worked together. Drawing a system architecture and data flow diagram helped me visualize their interactions and better understand the serverless architecture.

## Day 4 - 21/5: Designing the System Architecture

**Tasks Completed:** Together with my teammates, I analyzed the project requirements and designed the overall system architecture. We identified the main components of the system, including the frontend application, Amazon API Gateway, AWS Lambda, Amazon Cognito, Amazon DynamoDB, and Amazon S3. We also documented the data flow between these services.

**Knowledge Gained:** I learned that designing a well-structured system architecture before implementation is essential for building scalable, maintainable, and high-performance applications. Careful planning also simplifies future development and maintenance.

**Achievements:** Our team completed the initial architecture diagram and agreed on the implementation strategy for the upcoming development phases.

**Challenges and Lessons Learned:** Selecting the most appropriate AWS service for each system component required careful analysis. I learned that prioritizing serverless services can significantly reduce infrastructure management effort while improving scalability.

## Day 5 - 22/5: Reviewing Knowledge and Preparing for Development

**Tasks Completed:** I reviewed all the concepts covered during the week and verified the functionality of AWS Lambda, Amazon API Gateway, and Amazon DynamoDB. I also updated the project's technical documentation, revised the architecture diagram based on team feedback, and prepared the development environment for implementing the project's core business features in the following week.

**Knowledge Gained:** I reinforced my understanding of AWS serverless architecture and learned how AWS Lambda, Amazon API Gateway, Amazon Cognito, and Amazon DynamoDB work together to build modern web applications.

**Achievements:** I completed the development environment setup, gained a comprehensive understanding of the project's architecture, and was fully prepared to begin implementing the system's business functionalities.

**Challenges and Lessons Learned:** After working with several AWS services throughout the week, I realized that regularly reading the official AWS documentation and practicing in the AWS Management Console are the most effective ways to understand each service. I also improved my teamwork and communication skills by collaborating closely with my teammates to finalize technical decisions.