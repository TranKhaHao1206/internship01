---
title: "Week 2"
date: 2026-04-27
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

**Timeline:** 27/4 → 1/5 (5 working days)

## Day 1 - 27/4: AWS IAM Fundamentals

**Tasks Completed:** I started the second week by studying AWS Identity and Access Management (IAM). I explored the core IAM components, including IAM Users, IAM Groups, IAM Roles, and IAM Policies. I also created several test IAM Users to observe the differences between the Root Account and IAM Users, allowing me to better understand how AWS manages identities and permissions.

**Knowledge Gained:** I learned that IAM is AWS's centralized identity and access management service. The Root Account has full administrative access to all AWS resources and should only be used when absolutely necessary. In contrast, IAM Users are created for administrators and regular users to perform daily tasks securely.

**Achievements:** I successfully distinguished the roles of the Root Account and IAM Users and created multiple IAM Users for hands-on practice.

**Challenges and Lessons Learned:** Initially, I was confused about the differences between the Root Account and IAM Users. After practicing in the AWS Management Console, I realized that using IAM Users significantly improves security and simplifies access management.

## Day 2 - 28/4: Managing IAM Groups and Policies

**Tasks Completed:** I continued studying IAM Groups and IAM Policies. I created multiple Groups with different permission levels and assigned Users to them to observe how permissions are inherited. I also examined the structure of JSON-based IAM Policies, including fields such as Version, Effect, Action, Resource, and Condition.

**Knowledge Gained:** I learned that IAM Policies are collections of permissions written in JSON format. IAM Groups allow administrators to manage permissions for multiple users simultaneously instead of configuring each user individually, making system administration much more efficient.

**Achievements:** I successfully created IAM Groups, attached appropriate Policies to each Group, and understood the basic structure of an IAM Policy document.

**Challenges and Lessons Learned:** Reading JSON Policies was initially challenging because of their complexity. I found that studying each field individually while referring to the AWS documentation made it much easier to understand their purpose.

## Day 3 - 29/4: IAM Roles and the Principle of Least Privilege

**Tasks Completed:** I studied IAM Roles and learned how they differ from IAM Users. I created IAM Roles for AWS services and explored common use cases involving Amazon EC2, AWS Lambda, and other AWS services. I also studied the Principle of Least Privilege and its importance in cloud security.

**Knowledge Gained:** I learned that IAM Roles do not represent individual users. Instead, they provide temporary permissions to AWS services or users when needed. The Principle of Least Privilege minimizes security risks by granting only the permissions required to perform specific tasks.

**Achievements:** I successfully created basic IAM Roles and learned when to use IAM Users, Groups, or Roles in different scenarios.

**Challenges and Lessons Learned:** Determining the minimum required permissions for each Role was not straightforward. I learned that it is best practice to start with minimal permissions and expand them only when necessary.

## Day 4 - 30/4: AWS Regions, Availability Zones, and Edge Locations

**Tasks Completed:** I studied AWS's global infrastructure, including Regions, Availability Zones (AZs), and Edge Locations. I learned how to choose an appropriate Region based on geographic location, network latency, and application deployment requirements.

**Knowledge Gained:** I learned that an AWS Region is a geographic area where AWS services are deployed. Each Region consists of multiple independent Availability Zones to ensure high availability and fault tolerance. Edge Locations are used by AWS content delivery services to improve performance by caching content closer to end users.

**Achievements:** I gained a clear understanding of how to select an appropriate AWS Region and the role of Availability Zones in designing highly available systems.

**Challenges and Lessons Learned:** At first, I found it difficult to distinguish between Regions and Availability Zones. After reviewing AWS architecture diagrams, I understood how these components work together within AWS's global infrastructure.

## Day 5 - 1/5: IAM Review and Hands-on Practice

**Tasks Completed:** I reviewed all the IAM concepts covered throughout the week and practiced creating IAM Users, Groups, Roles, and Policies using the AWS Management Console. I also tested different permission scenarios to better understand AWS's access control mechanisms.

**Knowledge Gained:** I reinforced my understanding of IAM and gained deeper insight into access management within cloud environments. I also recognized the importance of applying the Principle of Least Privilege in real-world cloud systems.

**Achievements:** I successfully completed the fundamental IAM exercises and became confident in creating and managing IAM Users, Groups, Roles, and Policies.

**Challenges and Lessons Learned:** I realized that establishing clear naming conventions for resources and organizing IAM Policies properly makes system administration much easier as the number of users and resources grows.
