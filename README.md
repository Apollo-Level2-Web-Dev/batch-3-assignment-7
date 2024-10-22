# Assignment-7 (PostgreSQL)

**Assignment Description**  
In this assignment, you will work with PostgreSQL, a powerful open-source relational database management system. Your task involves creating 03 tables based on the provided sample data and then writing and executing queries to perform various database operations such as creating, reading, updating, and deleting data. Additionally, you will explore concepts like LIMIT and OFFSET, JOIN operations, GROUP BY, aggregation, and LIKE.

---

**Instructions:**

1. **Database Setup:**

   -  Install PostgreSQL on your system if not already installed.
   -  Create a fresh database titled "university_db" or any other appropriate name.

2. **Table Creation:**

   **Create a "students" table with the following fields:**

   -  `student_id (Primary Key)`: Integer, unique identifier for students.
   -  `student_name`: String, representing the student's name.
   -  `age`: Integer, indicating the student's age.
   -  `email`: String, storing the student's email address.
   -  `frontend_mark`: Integer, indicating the student's frontend assignment marks.
   -  `backend_mark`: Integer, indicating the student's backend assignment marks.
   -  `status`: String, storing the student's result status.

   **Create a "courses" table with the following fields:**

   -  `course_id (Primary Key)`: Integer, unique identifier for courses.
   -  `course_name`: String, indicating the course's name.
   -  `credits`: Integer, signifying the number of credits for the course.

   **Create an "enrollment" table with the following fields:**

   -  `enrollment_id (Primary Key)`: Integer, unique identifier for enrollments.
   -  `student_id (Foreign Key)`: Integer, referencing `student_id` in the "Students" table.
   -  `course_id (Foreign Key)`: Integer, referencing `course_id` in the "Courses" table.

---

### Sample Data

**Insert the following sample data into the "students" table:**

| student_id | student_name | age | email              | frontend_mark | backend_mark | status |
| ---------- | ------------ | --- | ------------------ | ------------- | ------------ | ------ |
| 1          | Sameer       | 21  | sameer@example.com | 48            | 60           | NULL   |
| 2          | Zoya         | 23  | zoya@example.com   | 52            | 58           | NULL   |
| 3          | Nabil        | 22  | nabil@example.com  | 37            | 46           | NULL   |
| 4          | Rafi         | 24  | rafi@example.com   | 41            | 40           | NULL   |
| 5          | Sophia       | 22  | sophia@example.com | 50            | 52           | NULL   |
| 6          | Hasan        | 23  | hasan@gmail.com    | 43            | 39           | NULL   |

**Insert the following sample data into the "courses" table:**

| course_id | course_name | credits |
| --------- | ----------- | ------- |
| 1         | Next.js     | 3       |
| 2         | React.js    | 4       |
| 3         | Databases   | 3       |
| 4         | Prisma      | 3       |

**Insert the following sample data into the "enrollment" table:**

| enrollment_id | student_id | course_id |
| ------------- | ---------- | --------- |
| 1             | 1          | 1         |
| 2             | 1          | 2         |
| 3             | 2          | 1         |
| 4             | 3          | 2         |

---

### Run SQL queries to complete the following tasks:

#### Query 1:

Insert a new student record with the following details:

-  Name: YourName
-  Age: YourAge
-  Email: YourEmail
-  Frontend-Mark: YourMark
-  Backend-Mark: YourMark
-  Status: NULL

**Note:** You can choose random values for the frontend_mark, backend_mark, and other fields (except NULL for the status).

#### Query 2:

Retrieve the names of all students who are enrolled in the course titled 'Next.js'.

**Sample Output:**

| student_name |
| ------------ |
| Sameer       |
| Zoya         |

#### Query 3:

Update the status of the student with the highest total (`frontend_mark + backend_mark`) to 'Awarded'.

#### Query 4:

Delete all courses that have no students enrolled.

#### Query 5:

Retrieve the names of students using a limit of 2, starting from the 3rd student.

**Sample Output:**

| student_name |
| ------------ |
| Nabil        |
| Rafi         |

#### Query 6:

Retrieve the course names and the number of students enrolled in each course.

**Sample Output:**

| course_name | students_enrolled |
| ----------- | ----------------- |
| Next.js     | 2                 |
| React.js    | 2                 |

#### Query 7:

Calculate and display the average age of all students.

**Sample Output:**

| average_age |
| ----------- |
| 22.33       |

#### Query 8:

Retrieve the names of students whose email addresses contain 'example.com'.

**Sample Output:**

| student_name |
| ------------ |
| Sameer       |
| Zoya         |
| Nabil        |
| Rafi         |
| Sophia       |

---

### Prepare the SQL code for table creation, sample data insertion, and the eight queries in a text document or your preferred format. Include comments explaining each query's purpose and functionality. Save your document as "PostgreSQL_Assignment.sql" or any other appropriate name.

---

### Questions (Answer 10 Questions):

1. What is PostgreSQL?
2. What is the purpose of a database schema in PostgreSQL?
3. Explain the primary key and foreign key concepts in PostgreSQL.
4. What is the difference between the VARCHAR and CHAR data types?
5. Explain the purpose of the WHERE clause in a SELECT statement.
6. What are the LIMIT and OFFSET clauses used for?
7. How can you perform data modification using UPDATE statements?
8. What is the significance of the JOIN operation, and how does it work in PostgreSQL?
9. Explain the GROUP BY clause and its role in aggregation operations.
10.   How can you calculate aggregate functions like COUNT, SUM, and AVG in PostgreSQL?
11.   What is the purpose of an index in PostgreSQL, and how does it optimize query performance?
12.   Explain the concept of a PostgreSQL view and how it differs from a table.

---

### Deadline:

-  60 Marks (24 October, 2024 Until 11.59 PM)
-  50 Marks (25 October, 2024 Until 11.59 PM)
-  30 Marks After 25 October, 2024 Until 11.59 PM

---

### Submission:

Submit only the GitHub repository link containing your solution file

---

**Important Note:** Attendance in this assignment is obligatory for all participants. As a follow-up, there will be two further assignments involving Prisma and PostgreSQL backends, specifically tailored for individuals with aspirations of becoming proficient full-stack developers. Approach this task with a thorough perspective and a commitment to achieving excellence. Wishing you the best of luck in your endeavors!
