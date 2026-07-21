---
title: "Week 11"
date: 2026-06-29
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

**Timeline:** 29/6 → 5/7 (5 working days)

## Day 1 - 29/6: Designing Test Cases and Planning System Testing

**Tasks Completed:** I began the system testing phase by analyzing the completed features and designing a comprehensive set of test cases. I created test scenarios for key functionalities, including user authentication, incident management, evidence management, role-based access control, reporting, and the AI Assistant. I also prepared a testing plan to ensure every feature would be thoroughly evaluated before the final demonstration.

**Knowledge Gained:** I learned that a well-designed test case should clearly define the testing steps, input data, expected results, and actual outcomes. A structured testing plan helps ensure that all functional and non-functional requirements are verified systematically.

**Achievements:** I completed the primary test case documentation for the core modules of the system and finalized the testing schedule with my teammates.

**Challenges and Lessons Learned:** Designing effective test cases required considering both valid and invalid user behaviors. I learned to approach testing from the user's perspective in order to create more realistic and comprehensive scenarios.

## Day 2 - 30/6: Testing Authentication and CRUD Operations

**Tasks Completed:** I tested the authentication module implemented with Amazon Cognito, including user login, logout, JWT token validation, and role-based authorization. Afterward, I verified all CRUD operations for Incident and Evidence management to ensure that data was processed correctly through both the frontend and backend.

**Knowledge Gained:** I learned that software testing should verify not only functional correctness but also security, authorization, and data integrity. I also gained additional experience using Postman to validate REST APIs independently from the web interface.

**Achievements:** The authentication process and CRUD operations performed reliably, with data being stored, updated, retrieved, and deleted correctly according to the system requirements.

**Challenges and Lessons Learned:** Some APIs initially returned unclear error messages when JWT tokens expired. I improved the application's error handling by providing more informative responses that help users understand authentication issues.

## Day 3 - 1/7: Testing Evidence Upload, Reports, and AI Assistant

**Tasks Completed:** I continued testing the Evidence Upload functionality using various file types, including images, PDF documents, and log files. I also evaluated the Report generation feature and the AI Assistant to verify that the system performed correctly under realistic usage scenarios.

**Knowledge Gained:** I learned that testing different input types helps identify issues related to file validation, upload limitations, and exception handling. I also recognized that AI-powered features should be evaluated using a wide variety of user questions to measure response quality and reliability.

**Achievements:** The Evidence Upload and Report generation features worked reliably. The AI Assistant successfully responded to questions related to the system's supported knowledge domain.

**Challenges and Lessons Learned:** Uploading large files increased processing time noticeably. I learned the importance of validating file size limitations and optimizing file transfer operations to Amazon S3 for better performance.

## Day 4 - 2/7: Recording and Resolving System Defects

**Tasks Completed:** After completing the testing activities, I documented all identified defects and categorized them according to their severity levels. Together with my teammates, I analyzed the root causes, corrected the source code, and performed regression testing to confirm that the issues had been successfully resolved.

**Knowledge Gained:** I learned that an effective defect management process consists of identifying issues, documenting them, analyzing their causes, implementing fixes, and performing regression testing. Maintaining detailed defect records improves project tracking and helps prevent similar issues from recurring.

**Achievements:** Most identified issues were successfully resolved, resulting in a more stable and reliable system after regression testing.

**Challenges and Lessons Learned:** Some defects appeared only under specific conditions, making them difficult to reproduce. I realized that creating diverse testing scenarios is essential for identifying hidden issues before deployment.

## Day 5 - 3/7: Preparing Technical Documentation

**Tasks Completed:** I completed the project's technical documentation, including the API documentation, system architecture diagram, sequence diagrams, and use case diagrams. I documented each API endpoint, HTTP method, request parameters, response structure, and processing workflow. I also updated the architecture diagrams to accurately reflect the final implementation of the system.

**Knowledge Gained:** I learned that technical documentation is an essential component of every software project because it enables new team members to understand the system more quickly and supports future maintenance. Well-organized documentation also simplifies project handover and evaluation.

**Achievements:** I completed the technical documentation required for system testing, project evaluation, and the final project demonstration.

**Challenges and Lessons Learned:** Technical documentation should be maintained continuously throughout development rather than only at the end of the project. I realized that clear and up-to-date documentation significantly improves communication among team members, supervisors, and project stakeholders.