# Database Testing – Classroom Presence Platform

## 1. Overview

This section documents the database testing performed on the Classroom Presence Platform, a MERN-stack application that uses MongoDB for data storage.

The objective of database testing was to verify that important application operations were correctly reflected in the MongoDB database. The checks focused on user registration, password storage, course creation, enrollment approval, and subject deactivation.

Testing was performed using **MongoDB Compass** connected to the project's MongoDB Atlas database.

## 2. Objectives

- Verify that registered users are correctly stored in MongoDB.
- Check that user passwords are stored in hashed format rather than plain text.
- Verify that newly created courses are persisted correctly.
- Confirm that enrollment approval is reflected in the database.
- Verify that subject deactivation updates the record instead of permanently deleting it.

## 3. Tools and Technologies

| Tool | Purpose |
|---|---|
| MongoDB Compass | Database inspection and verification |
| MongoDB Atlas | Cloud-hosted MongoDB database |
| MongoDB | NoSQL database |
| Classroom Presence Platform | Application under test |

## 4. Testing Scope

The following collections were inspected:

- `users`
- `courses`
- `enrollments`
- `subjects`

Five database test cases were executed to validate the persistence of important application data.

**Total Test Cases:** 5  
**Passed:** 5  
**Failed:** 0  

## 6. Key Observations

1. Registered user information was successfully stored in the `users` collection.
2. The password field contained a bcrypt-style hash instead of a plain-text password.
3. Course details, including the course name, course ID, description, and owner reference, were correctly persisted.
4. The approved enrollment record contained the expected approved status, student reference, course reference, and reviewer information.
5. Subject deactivation was implemented as a soft delete. The subject document remained in the database with `isActive` set to `false`.

## 7. Conclusion

Database testing confirmed that all five selected data-persistence checks passed successfully.

The verification demonstrated that important application operations, including user registration, course creation, enrollment approval, and subject deactivation, were correctly reflected in MongoDB.

This testing helped improve understanding of database validation, document structure, field relationships, ObjectId references, password hashing, and soft deletion.
