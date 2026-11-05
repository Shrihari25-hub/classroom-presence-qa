# Classroom Presence Platform – QA Testing Portfolio

## 1. Project Overview

This repository contains the Quality Assurance (QA) testing documentation and test evidence for the **Classroom Presence Platform**, a MERN-stack web application designed to manage classroom attendance and student presence verification.

The purpose of this project was to gain practical experience in software testing by performing manual website testing, API testing, API automation, and database validation on an actual application.

The testing activities focused on validating application functionality, verifying API responses, identifying defects, automating selected API scenarios, and checking whether application data was correctly stored in MongoDB.

## 2. Application Under Test

**Project:** Classroom Presence Platform

**Technology Stack:**
- Frontend: React.js
- Backend: Node.js and Express.js
- Database: MongoDB
- API Testing: Postman
- Database Validation: MongoDB Compass
- Database Hosting: MongoDB Atlas

## 3. Testing Objectives

- Validate the application's major functionalities through manual website testing.
- Verify API endpoints, HTTP methods, status codes, and response data.
- Test positive and negative scenarios.
- Identify and document unexpected application behaviour.
- Automate selected API test scenarios using Postman.
- Verify database records and data persistence using MongoDB Compass.
- Build practical knowledge of software testing and defect identification.

## 4. Testing Activities

The following testing activities were performed:

| Testing Activity | Description |
|---|---|
| Test Planning | Defined testing objectives, scope, and scenarios |
| Manual Website Testing | Tested application functionality, user workflows, form validations, course management, and attendance features |
| Manual API Testing | Executed API test cases covering authentication, courses, enrollments, and subjects |
| API Automation | Automated selected API requests using Postman Collection Runner |
| Database Testing | Verified stored records and data changes in MongoDB |

## 5. Testing Summary

### 5.1 Manual Website Testing

Manual functional testing was performed on the Classroom Presence Platform to verify its major features, user workflows, and application behaviour.

- Total manual test cases: 38
- Passed: 35
- Failed: 3
- Pass percentage: 92.11%

The testing identified three issues related to missing required-field indicators, duplicate course creation, and the inability to export only selected attendance records.

### 5.2 Manual API Testing

- Total manual API test cases: 45
- Passed: 44
- Failed: 1
- Pass percentage: 97.78%

The failed test identified an issue where registration with a password that was too short returned HTTP 500 instead of the expected HTTP 400.

### 5.3 API Automation

Selected API requests were automated using Postman test scripts and Collection Runner.

- Automated requests: 8
- Total assertions: 29
- Passed assertions: 29
- Failed assertions: 0
- Collection Runner iterations: 1

### 5.4 Database Testing

Database validation was performed using MongoDB Compass to verify data persistence and database operations.

- Total database test cases: 5
- Passed: 5
- Failed: 0
- Pass percentage: 100%

## 6. Tools Used

| Tool | Purpose |
|---|---|
| Postman | Manual API testing and API automation |
| MongoDB Compass | Database inspection and validation |
| MongoDB Atlas | Cloud-hosted database |
| Microsoft Excel | Test case documentation and test reports |
| Git | Version control |
| GitHub | Source code and QA portfolio documentation |

## 7. Detailed Documentation

Explore the following sections for detailed testing documentation:

- **[Test Plan](test-plan/README.md)** – Testing objectives, scope, approach, and planning.
- **[API Testing](api-testing/README.md)** – Manual API testing results, Postman automation, and identified issues.
- **[Database Testing](api-testing/database-testing/README.md)** – MongoDB database validation and test results.

## 8. Key Learnings

Through this project, I gained practical experience in:

- Understanding software testing fundamentals and test planning.
- Writing and executing manual test cases.
- Performing functional testing of web applications.
- Testing REST APIs using different HTTP methods.
- Validating HTTP status codes and JSON responses.
- Testing positive and negative scenarios.
- Using Postman variables and Bearer Token authentication.
- Writing Postman test scripts and assertions.
- Executing automated API collections using Collection Runner.
- Inspecting MongoDB documents and ObjectId references.
- Understanding password hashing and soft deletion.
- Documenting test results and identifying application defects.

## 9. Conclusion

This project provided hands-on experience in manual website testing, manual API testing, basic API automation, and database validation.

It helped develop a practical understanding of the software testing lifecycle, test case execution, API validation, data persistence, defect identification, and test documentation.

This portfolio represents my practical learning and application of QA concepts through testing a real-world academic software project.
