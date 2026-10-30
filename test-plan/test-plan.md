# Test Plan – Classroom Presence Platform

## 1. Introduction

The Classroom Presence Platform is a web-based attendance management application designed to help teachers manage courses and monitor student attendance.

The purpose of testing is to verify that the application works as expected, identify defects, and ensure that its major functionalities operate correctly.

## 2. Testing Objectives

The main objectives of testing are:

- Verify that users can register and log in successfully.
- Verify role-based access for teachers and students.
- Validate course creation and course management functionality.
- Verify attendance marking and attendance record management.
- Validate attendance history and data display.
- Verify attendance export functionality.
- Identify UI, functional, security and usability issues.
- Ensure that application data is handled consistently.

## 3. Scope of Testing

### 3.1 In Scope

The following modules are included in this testing activity:

| Module | Testing Coverage |
|---|---|
| Authentication | Registration, login and logout |
| User Interface | Page loading, navigation and form validation |
| Role-Based Access | Teacher and student permissions |
| Course Management | Course creation and duplicate course handling |
| Attendance Management | Attendance marking and attendance records |
| Attendance History | Viewing and validating attendance history |
| Export Functionality | Downloading and validating attendance reports |
| Security | Basic authorization and access-control checks |
| Usability | Basic navigation and user experience |

### 3.2 Out of Scope

- Performance and load testing.
- Automated UI testing.
- API testing, which is maintained separately using Postman.
- Production database testing.
- Mobile application testing.

## 4. Testing Approach

The project will primarily be tested using manual testing techniques.

The following testing types will be performed:

- **Functional Testing:** Verify that application features work according to expected requirements.
- **UI Testing:** Verify the layout, visibility and behaviour of application elements.
- **Positive Testing:** Verify application behaviour with valid inputs.
- **Negative Testing:** Verify application behaviour with invalid or unexpected inputs.
- **Validation Testing:** Verify mandatory fields and input restrictions.
- **Regression Testing:** Recheck existing functionality after changes or fixes.
- **Basic Security Testing:** Verify authentication and role-based access restrictions.
- **Data Validation Testing:** Verify that attendance and course information is displayed and maintained consistently.

## 5. Test Environment

| Environment | Details |
|---|---|
| Application | Classroom Presence Platform |
| Application URL | https://classroom-presence-platform.vercel.app/login |
| Testing Type | Manual Testing |
| Operating System | Windows |
| Browser | Google Chrome |
| API Testing Tool | Postman |
| Database | MongoDB |

## 6. Entry Criteria

Testing can begin when:

- The application is accessible.
- Required application modules are available.
- Test scenarios and test cases are prepared.
- Required test accounts and test data are available.
- The testing environment is ready.

## 7. Exit Criteria

Testing can be considered complete when:

- All planned test cases have been executed or their status documented.
- Actual results have been recorded.
- Failed test cases have been documented.
- Identified defects have been recorded.
- Test execution results have been summarized.

## 8. Test Deliverables

The following deliverables will be maintained in the QA repository:

- Test Plan
- Test Case Report

## 9. Risks and Limitations

- Some application features may change during testing.
- Test results may depend on the availability of accounts and data.
- Testing is limited to the available application functionality and the defined test scope.

## 10. Conclusion

This test plan provides the approach and scope for manually testing the Classroom Presence Platform.

Testing will focus on verifying the application's major functionalities, identifying defects, validating user interactions and ensuring that the application behaves as expected.
