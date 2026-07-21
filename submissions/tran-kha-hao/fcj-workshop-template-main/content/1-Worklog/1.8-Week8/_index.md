---
title: "Week 8"
date: 2026-06-08
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

**Timeline:** 8/6 → 14/6 (5 working days)

## Day 1 - 8/6: Initializing the ReactJS Project

**Tasks Completed:** I began developing the frontend of the Incident Response Management System (IRMS) using ReactJS. I initialized the project and organized the directory structure into modules such as Components, Pages, Services, and Assets. I also installed the required libraries, including React Router, Axios, and Material UI, to support frontend development.

**Knowledge Gained:** I learned that ReactJS is a JavaScript library for building user interfaces using a component-based architecture. Breaking the interface into reusable components makes the codebase easier to maintain, extend, and reuse as the application grows.

**Achievements:** I successfully initialized the ReactJS project and established a well-organized folder structure suitable for the project's scale.

**Challenges and Lessons Learned:** Initially, I was unsure how to organize the project structure effectively. After reviewing several widely used React project architectures, I selected a clear and maintainable structure that supports long-term development.

## Day 2 - 9/6: Designing the Dashboard Interface

**Tasks Completed:** I developed the Dashboard interface to provide an overview of incidents within the system. The dashboard displays key information such as the total number of incidents, their processing status, severity levels, and other statistical summaries. I used Material UI to create a consistent and user-friendly interface.

**Knowledge Gained:** I learned that the dashboard serves as the primary overview page, enabling administrators to quickly monitor the system's status. Presenting information visually helps users identify critical issues and make faster decisions during incident response.

**Achievements:** I completed the Dashboard interface with essential statistical widgets and a clean, well-structured layout.

**Challenges and Lessons Learned:** Designing an effective dashboard requires balancing clarity and usability. I learned to prioritize the most important information and place it in highly visible areas of the interface.

## Day 3 - 10/6: Developing the Incident List and Incident Detail Pages

**Tasks Completed:** I developed the Incident List and Incident Detail pages. The Incident List displays incidents in a table containing information such as the incident title, severity level, status, and creation date. Selecting an incident navigates the user to the Incident Detail page, where detailed information is displayed.

**Knowledge Gained:** I learned how to manage application data using React State and Props, as well as how to navigate between pages using React Router. I also gained experience displaying dynamic data retrieved from backend APIs.

**Achievements:** I successfully completed the two primary application screens and implemented navigation between them.

**Challenges and Lessons Learned:** Managing application state across multiple components became increasingly complex as the interface grew. I learned that breaking the interface into smaller reusable components and passing data efficiently improves maintainability.

## Day 4 - 11/6: Designing the Timeline and Evidence Upload Interface

**Tasks Completed:** I continued developing the Timeline interface to display the chronological history of incident handling. I also created the Evidence Upload interface, allowing users to upload log files, images, and PDF documents related to incidents.

**Knowledge Gained:** I learned that a timeline provides administrators with a clear view of the complete incident response process. I also studied how to use the FormData object in React to upload files through REST APIs.

**Achievements:** I completed both the Timeline interface and the Evidence Upload page with all required input fields and user interactions.

**Challenges and Lessons Learned:** Implementing file uploads required validating file types and file sizes before sending them to the server. I added validation messages to provide clear feedback whenever users attempted invalid uploads.

## Day 5 - 12/6: Connecting the Frontend with Amazon API Gateway and Amazon Cognito

**Tasks Completed:** I integrated the ReactJS frontend with the REST APIs through Amazon API Gateway. I also integrated Amazon Cognito for user authentication by attaching JWT tokens to API requests. Finally, I tested the complete login workflow and verified data retrieval from the backend services.

**Knowledge Gained:** I learned how to use Axios to send HTTP requests to Amazon API Gateway and include JWT tokens in the Authorization header for secure API access. I also gained a deeper understanding of communication between the frontend and backend in a serverless architecture.

**Achievements:** The ReactJS application successfully authenticated users through Amazon Cognito, invoked backend APIs, and displayed incident data retrieved from the system.

**Challenges and Lessons Learned:** During API integration, I encountered Cross-Origin Resource Sharing (CORS) issues and token expiration problems. After updating the API Gateway configuration and implementing token handling mechanisms, the application became more stable. I realized that thoroughly testing the complete frontend-backend workflow is essential for providing a reliable user experience.