# Classroom Presence Platform – API Testing

## Project Overview

This repository contains the API testing documentation and Postman automation performed for the **Classroom Presence Platform**, a MERN-stack application designed to manage classroom attendance and presence verification.

The purpose of this testing activity was to validate API functionality, verify expected HTTP responses, test authentication and authorization, check error handling, and automate selected API test scenarios using Postman.

Testing was performed against the locally running backend.

## Testing Objectives

- Validate API endpoints using Postman.
- Verify successful API operations and error responses.
- Test authentication and role-based authorization.
- Validate request data and response structures.
- Identify unexpected API behaviour.
- Automate selected test scenarios using Postman test scripts.
- Execute automated requests using the Postman Collection Runner.

## Tools and Technologies

| Tool | Purpose |
|---|---|
| Postman | API testing and automation |
| Node.js | Backend runtime |
| Express.js | REST API framework |
| MongoDB | Database |
| JavaScript | Postman test scripts |
| Excel | Manual test case documentation |
| Git and GitHub | Version control and documentation |

## Testing Scope

The following API modules were covered:

| Module | Test Cases |
|---|---:|
| Authentication | 14 |
| Courses | 15 |
| Enrollments | 11 |
| Subjects | 5 |
| **Total** | **45** |

### 1. Authentication

Tested scenarios included:

- User registration with valid details.
- Duplicate email registration.
- Missing required registration fields.
- Invalid user role.
- Password validation.
- Login with valid credentials.
- Login with incorrect credentials.
- Login with an unregistered email.
- Missing login fields.
- Retrieving the authenticated user's profile.
- Accessing protected endpoints without a token.
- Invalid or malformed authentication tokens.
- Face embedding validation.

### 2. Courses

Tested scenarios included:

- Creating a course with valid details.
- Missing course name or course ID.
- Duplicate course ID.
- Creating a course without an optional description.
- Retrieving courses belonging to the authenticated teacher.
- Retrieving a course using its course ID.
- Handling an invalid course ID.
- Updating course details.
- Accessing protected endpoints without authentication.
- Deleting a course as its owner.
- Preventing unauthorized course deletion.
- Adding a co-teacher.
- Handling an invalid co-teacher email.
- Removing a co-teacher.

### 3. Enrollments

Tested scenarios included:

- Submitting a valid student enrollment request.
- Requesting enrollment for an invalid course.
- Preventing duplicate enrollment requests.
- Retrieving the student's enrollments.
- Retrieving pending enrollment requests as a teacher.
- Retrieving approved students in a course.
- Approving an enrollment request.
- Rejecting an enrollment request.
- Preventing unauthorized enrollment review.
- Handling an invalid enrollment ID.
- Preventing students from accessing teacher-only endpoints.

### 4. Subjects

Tested scenarios included:

- Creating a subject under an authorized course.
- Preventing unauthorized subject creation.
- Updating subject details.
- Regenerating an invitation token.
- Deactivating a subject.

## Manual API Testing Results

A total of 45 manual API test cases were executed and documented.

| Result | Count |
|---|---:|
| Passed | 44 |
| Failed | 1 |
| Total | 45 |

The detailed test case report is available in:

`Classroom_Presence_API_Test_Cases.xlsx`

## Postman Automation

After completing manual API testing, selected important API requests were automated using Postman test scripts.

The following requests were included in the automation suite:

1. Verify Backend Health
2. Login
3. Get Current User
4. Create Course – Automation
5. Create Course – Duplicate ID
6. Get My Courses
7. Student Enrollment Request
8. Approve Enrollment

### Automation Features

- HTTP status code validation.
- Response body validation.
- User details verification.
- Authentication token extraction.
- Environment variable usage.
- Dynamic course ID generation.
- Dynamic enrollment ID extraction.
- Enrollment status verification.
- Sequential execution using Collection Runner.

### Automation Results

| Result | Count |
|---|---:|
| Passed Assertions | 29 |
| Failed Assertions | 0 |
| Total Assertions | 29 |

**Collection Runner Result: 29 Passed, 0 Failed.**

## Known Issue Identified

During manual API testing, one issue was identified:

**Test Case ID:** AUTH_TC_005

**Scenario:** User registration with a password shorter than the required minimum length.

**Expected Result:** The API should return HTTP 400 Bad Request with an appropriate validation message.

**Actual Result:** The API returned HTTP 500 Internal Server Error due to a Mongoose validation error.

**Status:** Failed

This indicates that the password validation error is not being handled with the expected client-error response.

## Key Learnings

Through this testing activity, I gained practical experience in:

- Understanding REST API testing.
- Working with HTTP methods and status codes.
- Sending requests with JSON payloads.
- Testing authentication using JWT tokens.
- Understanding bearer-token authorization.
- Validating API responses using JavaScript assertions.
- Working with Postman environment variables.
- Extracting and reusing dynamic response values.
- Automating API test scenarios.
- Executing collections using Postman Collection Runner.
- Documenting test cases and identifying API defects.

## Conclusion

This project helped me gain hands-on experience in manual API testing and basic API test automation using Postman.

A total of 45 manual test cases were executed across four modules, and eight selected API requests were included in the automation suite, resulting in 29 passing assertions.

The testing activity also helped identify an API validation-handling issue during user registration.
