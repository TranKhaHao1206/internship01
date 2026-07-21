---
title: "Week 6"
date: 2026-05-25
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

**Timeline:** 25/5 → 31/5 (5 working days)

## Day 1 - 25/5: Studying Amazon API Gateway

**Tasks Completed:** I began studying Amazon API Gateway to build REST APIs for the Incident Response Management System (IRMS). I explored the core components of API Gateway, including APIs, Resources, Methods, Stages, and Deployments. I also created my first REST API and tested it using Postman.

**Knowledge Gained:** I learned that Amazon API Gateway serves as the entry point for client requests, handling authentication, routing requests to AWS Lambda, and returning responses to applications. It provides centralized API management, improves scalability, and enhances security.

**Achievements:** I successfully created my first REST API in Amazon API Gateway and verified its functionality through Postman.

**Challenges and Lessons Learned:** Initially, I found it difficult to understand the relationship between Resources and Methods in API Gateway. After practicing with multiple API configurations, I gained a clearer understanding of how REST APIs should be organized.

## Day 2 - 26/5: Developing REST APIs for the IRMS Project

**Tasks Completed:** I developed REST APIs for the IRMS project, including endpoints for retrieving incidents, creating new incidents, updating existing records, and deleting data. I designed these endpoints according to RESTful principles to ensure maintainability and scalability.

**Knowledge Gained:** I learned the fundamental principles of REST API design, including the appropriate use of HTTP methods such as GET, POST, PUT, and DELETE, as well as best practices for organizing resource URLs.

**Achievements:** I completed the core REST API endpoints required for incident management and prepared them for integration with AWS Lambda.

**Challenges and Lessons Learned:** I realized that API design should be carefully planned from the beginning to avoid unnecessary modifications during later stages of development. Consistent endpoint naming significantly improves maintainability.

## Day 3 - 27/5: Configuring Routes, Methods, and Integrating with AWS Lambda

**Tasks Completed:** I configured API Gateway routes and HTTP methods, then integrated each endpoint with the AWS Lambda functions developed during the previous week. I tested data transmission between the client, API Gateway, and Lambda using Postman to verify that the serverless workflow functioned correctly.

**Knowledge Gained:** I learned the complete request lifecycle in a serverless architecture: Client → API Gateway → AWS Lambda → Amazon DynamoDB → Response. I also gained experience working with the Lambda event object for handling incoming requests.

**Achievements:** All REST APIs successfully invoked the corresponding Lambda functions and returned responses in JSON format.

**Challenges and Lessons Learned:** During integration, API Gateway was initially unable to invoke the Lambda functions because the required execution permissions had not been configured. After updating the Lambda permissions and redeploying the API, the integration worked as expected.

## Day 4 - 28/5: Learning Amazon S3

**Tasks Completed:** I studied Amazon Simple Storage Service (Amazon S3) in preparation for implementing file storage in the IRMS project. I created an S3 bucket, configured access permissions, uploaded and downloaded sample files, and explored object management features within Amazon S3.

**Knowledge Gained:** I learned that Amazon S3 is a highly durable and scalable object storage service. I also understood how data is organized into buckets and objects, as well as the security best practices for managing files in cloud storage.

**Achievements:** I successfully created an Amazon S3 bucket and performed file upload, download, and deletion operations.

**Challenges and Lessons Learned:** At first, I encountered access issues caused by incorrect bucket permissions. I learned the importance of verifying both IAM Policies and Bucket Policies before deploying storage solutions.

## Day 5 - 29/5: Attending an AWS Workshop and Weekly Review

**Tasks Completed:** I attended an AWS technical workshop to learn more about cloud services and current serverless development practices. AWS experts shared practical experience in deploying production systems, optimizing cloud costs, and improving security. After the workshop, I reviewed the week's learning outcomes and updated the project's technical documentation.

**Knowledge Gained:** I gained a deeper understanding of serverless architectures, modern cloud design principles, and the process of selecting appropriate AWS services for real-world applications. I also benefited from practical insights shared by AWS professionals.

**Achievements:** I expanded my knowledge of the AWS ecosystem, completed the project's core REST APIs, and established a solid foundation for implementing business features in the following weeks.

**Challenges and Lessons Learned:** The workshop covered a large amount of technical content, so I documented the most important topics for further study. I realized that participating in professional events is an excellent way to stay updated with new technologies and improve cloud architecture design skills.