# Database Schema

## Students Table

  Column       Description
  ------------ --------------
  student_id   Primary key
  name         Student name
  department   Department
  email        Email
  phone        Phone number

## Teachers Table

  Column       Description
  ------------ ----------------
  teacher_id   Primary key
  name         Teacher name
  department   Department
  email        Email
  password     Login password

## Attendance Table

  Column          Description
  --------------- ------------------
  attendance_id   Primary key
  student_id      Foreign key
  date            Attendance date
  status          Present / Absent

## Assessments Table

  Column          Description
  --------------- -------------
  assessment_id   Primary key
  student_id      Foreign key
  subject         Subject
  marks           Marks
  grade           Grade
