---
title: "Week 9"
date: 2026-06-15
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

**Timeline:** 15/6 → 21/6 (5 working days)

## Day 1 - 15/6: Enhancing the Incident Monitoring Dashboard

**Tasks Completed:** I continued improving the Dashboard interface of the Incident Response Management System (IRMS). I added summary cards displaying the total number of incidents, incidents in progress, resolved incidents, and overdue incidents. I also refined the dashboard layout to help users quickly understand the current status of the system.

**Knowledge Gained:** I learned that an effective dashboard should not only display information but also help administrators make quick decisions. Organizing data based on priority improves visibility and enables faster incident response.

**Achievements:** The Dashboard successfully displays comprehensive system statistics and retrieves real-time data from the backend APIs.

**Challenges and Lessons Learned:** Displaying too many elements on a single screen can reduce readability. I learned to group related information together and organize the layout more effectively to improve user experience.

## Day 2 - 16/6: Implementing Incident Severity Classification

**Tasks Completed:** I developed the incident severity classification feature with three severity levels: Critical, High, and Medium. I updated the database schema by adding a severity field and modified the user interface to display different severity levels using color-coded labels.

**Knowledge Gained:** I learned that incident severity classification allows security teams to prioritize critical incidents, reducing overall risk and improving response efficiency.

**Achievements:** Users can now select the severity level when creating an incident, and the selected severity is displayed consistently on both the Dashboard and the Incident List.

**Challenges and Lessons Learned:** Initially, I stored severity values as plain strings, which made future expansion difficult. After discussing the design with my teammates, I standardized the data structure to improve scalability and maintainability.

## Day 3 - 17/06: Improving the User Interface

**Tasks Completed:** I reviewed the entire application interface and refined spacing, colors, icons, and layouts across the Dashboard, Incident List, and Incident Detail pages. I also added loading indicators and error messages to improve user interaction and provide better feedback during system operations.

**Knowledge Gained:** I learned that a user-friendly interface reduces operational errors and enables users to perform tasks more efficiently. Besides functionality, visual consistency and usability are essential for a successful web application.

**Achievements:** The application's interface became more consistent, easier to navigate, and more responsive across different screen sizes.

**Challenges and Lessons Learned:** Some interface components did not display properly on smaller screens. I gained practical experience applying responsive design techniques to ensure compatibility across multiple devices.

## Day 4 - 18/6: Testing the Incident Processing Workflow

**Tasks Completed:** I tested the complete incident management workflow, including incident creation, updating information, changing incident status, and completing incident resolution. I used both Postman and the web application to verify communication between the frontend and backend while documenting any issues discovered during testing.

**Knowledge Gained:** I learned that testing complete business workflows is more effective than testing isolated features because it reveals issues that only occur during real user interactions.

**Achievements:** I completed testing of the core application features and resolved several issues related to data presentation and incident status updates.

**Challenges and Lessons Learned:** Some bugs only appeared after performing multiple sequential operations. I learned the importance of creating comprehensive test scenarios that simulate real-world usage instead of testing individual functions independently.

## Day 5 - 19/6: Verifying User Authorization and Weekly Review

**Tasks Completed:** I verified the role-based authorization mechanism implemented in the IRMS project. I tested the permissions assigned to different roles, including Admin, Security Manager, Security Analyst, and Auditor, ensuring that each role had appropriate access to functions such as incident creation, incident editing, evidence uploading, and report viewing. At the end of the day, I summarized the week's progress and updated the project's technical documentation.

**Knowledge Gained:** I gained a deeper understanding of access control and the importance of protecting system resources through role-based authorization. I also reinforced the Least Privilege principle, ensuring that users receive only the permissions required to perform their responsibilities.

**Achievements:** The role-based access control system functioned according to the project design. Backend APIs were protected using Amazon Cognito JWT tokens, and the frontend correctly displayed features based on each user's assigned role.

**Challenges and Lessons Learned:** During testing, I discovered that some interface elements were still visible to users without sufficient permissions. After updating both frontend visibility rules and backend authorization checks, the application became more secure. I realized that verifying security at both the user interface and API levels is essential for building a reliable application.
