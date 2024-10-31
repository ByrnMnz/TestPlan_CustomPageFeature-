# QA TEST PLAN: CUSTOM PAGE TESTING FOR PLANNING CENTER PUBLISHING

## Project
This test plan project was requested during a job application process. I was given all creative freedom to showcase my analytical thinking and to provide complete test coverage for the Custom Page feature of the Planning Center's Publishing product.
The following link explains what the custom page feature does and how it works. 
https://pcopublishing.zendesk.com/hc/en-us/articles/360052458693-Create-a-Custom-Page

# Table of Contents

INTRODUCTION 

1.1 PURPOSE

1.2 SCOPE

1.3 TEAM MEMBERS

2 RISKS

3 TEST APPROACH 

3.1 TESTING OBJECTIVES

3.2 TEST SCOPE

3.3 TEST STRATEGY

4 TEST ENVIRONMENT

4.1 TEST CASES

4.1.1 Functional Tests

4.1.2 UI/UX Tests

4.1.3 Performance Tests

4.1.4 Cross-Browser Compatibility

4.1.5 Security Tests

5 MILESTONES & DELIVERABLES

5.1 TEST SCHEDULE

5.2 DELIVERABLES

6 ENTRY & EXIT CRITERIA

6.1 ENTRY CRITERIA

6.2 EXIT CRITERIA

# Introduction
## 1.1 Purpose:

The test plan has been created to communicate the test approach to all team members. Its purpose is to validate the functionality, performance, and security of the custom page developed by Planning Center Publishing. This document presents the scope, risks, test approaches, test environments, testing methods, milestones and deliverables, and a completion and exit strategy.

## 1.2 Scope:

This plan will cover functional testing, user acceptance testing (UAT), performance testing, cross-browser compatibility, security checks, and responsive testing on various devices and browsers.
Performance testing will be considered part of this project due to the large user base and concurrent users using the site hourly or daily.
Rewriting, moving, or archiving existing test cases from the existing Word documents will be revisited during future iterations as features are released. This will keep testing up to date with new updates and remove redundant testing to maintain SLA and feature release schedule.

## 1.3 Team Members:

| Role               | Name          | Responsibilities                                                    |
| ------------------ |:-------------:| ------------------------------------------------------------------- |
| QA Lead            | [Name]        | Define test plans, review test cases, and manage overall execution. |
| QA Engineer/Tester | [Name]        | Execute manual and automated tests and report defects.              |
| Developer          | [Name]        | Provide builds for testing and assist with bug fixes.               |
| UI/UX Designer     | [Name]        | Validate that the custom page adheres to design guidelines.         |
| Product Manager    | [Name]        | Ensure the custom page meets business and user requirements.        |
| DevOps Engineer    | [Name]        | Manage the test environment and deployment process.                 |

## Risks 

| Risk                                     | Impact                                                                                                          | Trigger                                                                          | Mitigation Stratagy                                                                                                               |
| ---------------------------------------  |:-------------------------------------------------------------------------------------------------------------:  | -------------------------------------------------------------------------------  | --------------------------------------------------------------------------------------------------------------------------------- |
| Page performance issues when under load  | Slow page load times or crashes during peak usage.                                                              | High traffic volume or inefficient resource handling.                            | Conduct early performance testing, optimize code, use caching, and CDN to improve performance.                                    |
| Security vulnerabilities.                | Exposure of sensitive data or compromise of the system.                                                         | Lack of proper input validation and insecure communication channels.             | Perform thorough security testing (e.g., penetration testing), validate with security experts, and use HTTPS.                     |
| Cross-browser compatibility              | Inconsistent user experience across different browsers.                                                         | Page elements render differently or break on specific browsers.	                |Test the custom page across all targeted browsers early in development.                                                            |
| Design inconsistencies                   | Poor user experience and potential usability issues.                                                            | Design elements appear differently than intended across devices.	                | Regularly validate design with the UI/UX team, ensuring alignment with style guides and responsive design.                        |
| Data loss during form submissions        | Loss of user input or incomplete data processing.                                                               | System crashes or errors during form submission.	                                | Use dummy test data, implement robust backup mechanisms, and log transactions to prevent and recover data loss.                   |
| Unclear or incomplete requirements       | Unclear or incomplete requirements                                                                              | Misinterpretation of requirements or incomplete documentation.                   | Review requirements with stakeholders, maintain a requirements traceability matrix, and clarify any ambiguities.                  |
| Deployment and environmental issues      | Features may not work as expected due to ecological differences.                                                | Misconfigured test environment and different software versions.                  | Maintain consistency between test and production environments and use CI pipelines for automated deployment.                      |
| Mobile Network Connectivity Issues       | Poor performance or broken functionality on slow or unstable mobile connections.                                | Users are accessing the page from mobile devices on unstable networks.           | Optimize for mobile performance (e.g., use lightweight assets) and implement offline fallback for critical functions.             |
| User Behavior Misalignment               | Custom page design may not align with the typical user workflow, leading to confusion.                          | Incorrect assumptions about how users will interact with the page.               | Conduct user testing and collect feedback from real users early to ensure the design matches user behavior and expectations.      |
| Feature Scope Creep                      | An overcomplicated design may confuse users and degrade performance.                                            | Adding too many features beyond the original scope without user validation.      | Use agile methodologies to manage scope, prioritize user-focused features, and regularly review the MVP (Minimum Viable Product). |
| Multiple Control Conflicts               | Multiple contributors might cause code conflicts or revert significant changes, impacting the page’s stability. | Poor version control management or multiple team members editing simultaneously. | Use a robust version control system (e.g., Git) to enforce clear commit/pull request processes and conduct regular code reviews.  |
| Unforeseen User-Generated Content Issues | Users may post inappropriate or harmful content (if user input is allowed).                                     | Insufficient content moderation or validation mechanisms.                        | Implement content moderation tools, set up filters to flag inappropriate content, and establish user-reporting mechanisms.        |






