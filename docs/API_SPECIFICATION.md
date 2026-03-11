# API Specification
## Jeenify – Backend Endpoints

This document outlines the core backend API endpoints used in the Jeenify system.

## Authentication

### POST /login
Authenticate teacher/admin login.

Request Body:
- email
- password

Response:
- success / failure
- session token (if implemented)

---

## Student Management

### POST /students
Add a new student.

Fields:
- name
- department
- email
- phone

### GET /students
Retrieve list of all students.

### GET /students/{id}
Retrieve specific student details.

### PUT /students/{id}
Update student information.

### DELETE /students/{id}
Delete a student.

---

## Attendance

### POST /attendance
Mark attendance for students.

Fields:
- student_id
- date
- status (Present / Absent)

### GET /attendance/{student_id}
Retrieve attendance history for a student.

---

## Assessments

### POST /assessments
Add marks for a student.

Fields:
- student_id
- subject
- marks

### GET /assessments/{student_id}
Retrieve assessment records for a student.

---

## Reports

### GET /reports/attendance
Generate attendance report.

### GET /reports/performance
Generate student performance report.