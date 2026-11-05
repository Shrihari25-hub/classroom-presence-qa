# Test Plan – Classroom Presence Platform

## 1. Introduction

The Classroom Presence Platform is a web-based attendance management application designed to help teachers manage courses, monitor student attendance and maintain attendance records.

The purpose of this testing activity is to verify that the application functions as expected, identify defects, validate API behaviour, check database operations and ensure that application data is handled consistently.

This test plan defines the scope, objectives, testing approach, environment and deliverables for the overall QA testing of the Classroom Presence Platform.

The testing activities include Manual Website Testing, Manual API Testing, API Automation Testing and Database Testing.

## 2. Testing Objectives

The main objectives of testing are:

- Verify that users can register and log in successfully.
- Verify role-based access for teachers and students.
- Validate course creation and course management functionality.
- Verify attendance marking and attendance record management.
- Validate attendance history and data display.
- Verify attendance export functionality.
- Validate API endpoints using positive and negative test scenarios.
- Verify API responses, HTTP status codes and authentication behaviour.
- Automate selected API test scenarios using Postman Collection Runner.
- Verify that important application data is correctly stored and maintained in MongoDB.
- Identify UI, functional, API, security and data-related issues.
- Ensure that application functionality and data handling behave as expected.

## 3. Scope of Testing

### 3.1 In Scope

The following modules and testing activities are included in this project:

| Module / Testing Activity | Testing Coverage |
|---|---|
| Authentication | Registration, login, logout and authentication validation |
| User Interface | Page loading, navigation and form validation |
| Role-Based Access | Teacher and student permissions |
| Course Management | Course creation, duplicate course handling and course retrieval |
| Attendance Management | Attendance marking and attendance records |
| Attendance History | Viewing and validating attendance history |
| Export Functionality | Downloading and validating attendance reports |
| Manual API Testing | API endpoint validation, request/response verification and HTTP status codes |
| API Authentication | Token-based authentication and authorization checks |
| API Negative Testing | Invalid inputs, missing fields and unauthorized requests |
| API Automation | Automated execution of selected API requests and assertions using Postman |
| Database Testing | Verification of user, course, enrollment and subject records in MongoDB |
| Data Integrity | Validation of stored records, relationships, status fields and data persistence |
| Security | Basic authentication and access-control checks |
| Usability | Basic navigation and user experience |

### 3.2 Out of Scope

The following testing activities are not included in this project:

- Performance and load testing.
- Stress and scalability testing.
- Automated UI testing.
- Full security penetration testing.
- Production database testing.
- Mobile application testing.
- Continuous automated testing through a CI/CD pipeline.

## 4. Testing Approach

The project uses a combination of manual and automated testing techniques.

The following testing approaches are included:

### 4.1 Manual Website Testing

The application interface and major functionalities will be tested manually.

Testing includes:

- Functional Testing: Verify that application features work according to expected requirements.
- UI Testing: Verify the layout, visibility and behaviour of application elements.
- Positive Testing: Verify application behaviour with valid inputs.
- Negative Testing: Verify application behaviour with invalid or unexpected inputs.
- Validation Testing: Verify mandatory fields and input restrictions.
- Regression Testing: Recheck existing functionality after changes or fixes.
- Basic Security Testing: Verify authentication and role-based access restrictions.
- Usability Testing: Verify basic navigation and user experience.

### 4.2 Manual API Testing

API endpoints will be tested using Postman.

Testing includes:

- Verify API endpoints using appropriate HTTP methods.
- Validate request payloads and response bodies.
- Verify HTTP status codes.
- Test valid and invalid input scenarios.
- Verify authentication and authorization behaviour.
- Validate error responses and input handling.
- Verify API behaviour for different user roles.

### 4.3 API Automation Testing

Selected API requests will be automated using Postman.

Testing includes:

- Execute selected API requests using Postman Collection Runner.
- Validate HTTP status codes and response data using assertions.
- Verify request execution and response behaviour.
- Review automated execution results.

### 4.4 Database Testing

Database records will be inspected using MongoDB Compass.

Testing includes:

- Verify user registration records.
- Verify password storage format.
- Verify course creation records.
- Verify enrollment approval records.
- Verify subject soft-deletion behaviour.
- Validate important fields, record relationships and data persistence.

## 5. Test Environment

The following tools and environments are used for testing:

| Environment / Tool | Details |
|---|---|
| Application | Classroom Presence Platform |
| Application URL | https://classroom-presence-platform.vercel.app/login |
| Operating System | Windows |
| Browser | Google Chrome |
| Manual Testing Tool | Web Browser |
| API Testing Tool | Postman |
| API Automation Tool | Postman Collection Runner |
| Database | MongoDB |
| Database Inspection Tool | MongoDB Compass |
| Backend Environment | Local development environment |
| Test Data | Dedicated teacher and student test accounts |

## 6. Entry Criteria

Testing can begin when:

- The application and required backend services are accessible.
- Required application modules are available.
- Test scenarios and test cases are prepared.
- Required test accounts and test data are available.
- The API endpoints are accessible.
- The testing tools and database environment are ready.

## 7. Exit Criteria

Testing can be considered complete when:

- All planned test cases have been executed or their status documented.
- Actual results have been recorded.
- Failed test cases have been documented.
- Identified defects have been recorded.
- Selected API automation requests have been executed.
- Database records have been verified for the planned test scenarios.
- Test execution results have been summarized.

## 8. Test Deliverables

The following deliverables are maintained in the QA repository:

- Project Test Plan.
- Manual Website Test Case Report.
- Manual API Test Case Report.
- Postman API Testing Collection.
- Postman Environment Configuration.
- Postman Collection Runner Execution Evidence.
- Database Test Case Report.
- API Testing Documentation.
- Database Testing Documentation.
- Identified Defects and Test Execution Results.

## 9. Risks and Limitations

- Some application features may change during testing.
- Test results may depend on the availability of accounts and test data.
- Testing is limited to the available application functionality and defined test scope.
- API automation covers selected requests and does not represent complete API automation.
- Database testing is limited to selected collections and records.
- Performance, load and advanced security testing are not included.

## 10. Conclusion

This test plan defines the overall testing strategy for the Classroom Presence Platform.

The QA project covers Manual Website Testing, Manual API Testing, API Automation Testing and Database Testing.

These activities aim to verify application functionality, validate API behaviour, inspect database operations, identify defects and assess the overall reliability of the application.
