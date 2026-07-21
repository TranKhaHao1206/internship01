---
title: "Week 7"
date: 2026-06-01
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

**Timeline:** 1/6 → 7/6 (5 working days)

## Day 1 - 01/6: Developing the Evidence Management Module

**Tasks Completed:** I began developing the Evidence Management module for the Incident Response Management System (IRMS). I analyzed the business requirements and identified the types of evidence that needed to be managed, including log files, images, PDF documents, and descriptive metadata. I then designed the data structure and processing workflow for the module.

**Knowledge Gained:** I learned the importance of evidence management in an incident response system. Proper storage and organization of digital evidence support incident investigation, forensic analysis, and compliance auditing. I also learned that separating metadata from file content improves system performance and simplifies data management.

**Achievements:** I completed the initial design of the Evidence Management module and identified all essential data fields required for storing and managing evidence.

**Challenges and Lessons Learned:** Defining the complete set of evidence attributes required reviewing technical documentation and discussing requirements with my teammates. I realized that thorough requirement analysis significantly reduces implementation changes during development.

## Day 2 - 2/6: Integrating Amazon S3 for Evidence Storage

**Tasks Completed:** I integrated Amazon S3 into the system to store evidence files. I created a dedicated S3 bucket for the project, organized the storage structure, and configured IAM Roles to allow AWS Lambda functions to securely access Amazon S3.

**Knowledge Gained:** I learned that Amazon S3 is better suited for storing large files than keeping them directly in a database. Storing only file metadata and object paths in Amazon DynamoDB improves system performance while reducing storage costs.

**Achievements:** The system successfully uploaded evidence files to Amazon S3 and stored the corresponding file references in Amazon DynamoDB.

**Challenges and Lessons Learned:** Initially, the Lambda functions could not upload files because of insufficient permissions. After updating the IAM Policy and verifying the Bucket Policy, the upload process worked correctly.

## Day 3 - 3/6: Supporting Multiple File Types

**Tasks Completed:** I enhanced the upload functionality to support multiple file formats, including images, log files, and PDF documents. I also implemented a file naming convention based on Incident IDs to prevent duplicate filenames and simplify future file retrieval.

**Knowledge Gained:** I learned that organizing Amazon S3 objects using logical folder structures and consistent naming conventions greatly improves file management at scale. I also studied file type validation techniques to ensure that only supported file formats can be uploaded.

**Achievements:** The upload feature successfully handled multiple file types, and uploaded files were stored in the correct Amazon S3 locations.

**Challenges and Lessons Learned:** During testing, I observed that large files required significantly more upload time. I learned the importance of implementing exception handling and progress indicators to improve the overall user experience.

## Day 4 - 4/6: Testing the Evidence Management Module

**Tasks Completed:** I performed comprehensive testing of the Evidence Management module, including creating evidence records, uploading files to Amazon S3, viewing stored evidence, and deleting obsolete data. I also collaborated with my teammates to verify the module's stability and reliability.

**Knowledge Gained:** I learned that testing each completed feature before system integration is essential for identifying issues related to permissions, data validation, and processing workflows. Early testing helps reduce integration problems in later development stages.

**Achievements:** The Evidence Management module functioned as expected, with evidence files successfully stored and retrieved from Amazon S3.

**Challenges and Lessons Learned:** Some issues occurred because user input validation was incomplete. I improved the upload process by adding additional validation steps before files were submitted to Amazon S3.

## Day 5 - 5/6: Exploring Additional AWS Services and Weekly Review

**Tasks Completed:** I spent time studying additional AWS services that could support the IRMS project, including Amazon CloudWatch for monitoring logs and system performance, AWS CloudTrail for auditing AWS account activities, and AWS Secrets Manager for securely storing sensitive information such as API keys and credentials. At the end of the day, I reviewed everything I had learned throughout the week and updated the project's technical documentation.

**Knowledge Gained:** I gained a deeper understanding of monitoring and security services within the AWS ecosystem. I learned that Amazon CloudWatch provides operational monitoring and logging, AWS CloudTrail records API activities for auditing purposes, and AWS Secrets Manager securely manages confidential application credentials.

**Achievements:** I expanded my knowledge of AWS services, completed the Evidence Management module, and established a solid foundation for developing the user interface during the following week.

**Challenges and Lessons Learned:** AWS provides a wide range of services with overlapping capabilities, making service selection an important design decision. I realized that studying the official AWS documentation and gaining hands-on experience are the most effective ways to understand the strengths and appropriate use cases of each service.