# Experiment 1: Entity-Relationship (ER) Diagram

## 🎯 Objective:
To understand and apply the concepts of ER modeling by creating an ER diagram for a real-world application.

## 📚 Purpose:
The purpose of this workshop is to gain hands-on experience in designing ER diagrams that visually represent the structure of a database including entities, relationships, attributes, and constraints.

---

## 🧪 Choose One Scenario:

### 🔹 Scenario 1: University Database
Design a database to manage students, instructors, programs, courses, and student enrollments. Include prerequisites for courses.

**User Requirements:**
- Academic programs grouped under departments.
- Students have admission number, name, DOB, contact info.
- Instructors with staff number, contact info, etc.
- Courses have number, name, credits.
- Track course enrollments by students and enrollment date.
- Add support for prerequisites (some courses require others).

---

### 🔹 Scenario 2: Hospital Database
Design a database for patient management, appointments, medical records, and billing.

**User Requirements:**
- Patient details including contact and insurance.
- Doctors and their departments, contact info, specialization.
- Appointments with reason, time, patient-doctor link.
- Medical records with treatments, diagnosis, test results.
- Billing and payment details for each appointment.

---

## 📝 Tasks:
1. Identify entities, relationships, and attributes.
2. Draw the ER diagram using any tool (draw.io, dbdiagram.io, hand-drawn and scanned).
3. Include:
   - Cardinality & participation constraints
   - Prerequisites for University OR Billing for Hospital
4. Explain:
   - Why you chose the entities and relationships.
   - How you modeled prerequisites or billing.

# ER Diagram Submission - Student Name
```
Name: Ashwin Akash M
Reference Number: 212223230024
```
## Scenario Chosen:
University / Hospital (choose one)

## ER Diagram:
![University Database](https://github.com/user-attachments/assets/e082608e-920c-427d-837e-cbd7d79ff5ce)


## Entities and Attributes:
1. Student: StudentID,Name,Gender,DOB,Email,Phone,Address
2. Instructor: InstructorID,Name,Phone,Email
3. Department: DepartmentID,Department Name,Head of Department
4. Course: CourseID,Course Name,Credits
5. Enrollment : EnrollmentID,EnrollmentDate,Grade
6. Schedule : ScheduleID,Day,Time
7. Classroom : ClassroomID,Building,Room Number,Capacity ...
## Relationships and Constraints:
1. Enrollment (StudentID,CourseID )
2. Course (DepartmentID, CourseID)
3. Instructor(InstructorID,CourseID)
4. Schedule(CourseID,ClassroomID) ...
## RESULT
Thus,we have created an E-R Diagram for the chosen scenario successfully defining necessary entities,attributes,relationships and constraints.
