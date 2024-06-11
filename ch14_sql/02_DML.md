Data Manipulation in SQL involves using Data Manipulation Language (DML) commands to query and modify data within database tables. The primary DML commands are `SELECT`, `INSERT`, `UPDATE`, and `DELETE`. Here’s a detailed explanation of each command with examples using a `students` table.

### 1. SELECT
Used to query data from a table.

#### Syntax
```sql
SELECT column1, column2, ...
FROM table_name
WHERE condition;
```

#### Example
Querying all students.
```sql
SELECT * FROM students;
```

Querying specific columns and applying a condition.
```sql
SELECT first_name, last_name, gpa
FROM students
WHERE gpa > 3.5;
```

### 2. INSERT
Used to add new rows to a table.

#### Syntax
```sql
INSERT INTO table_name (column1, column2, ...)
VALUES (value1, value2, ...);
```

#### Example
Inserting a new student.
```sql
INSERT INTO students (student_id, first_name, last_name, date_of_birth, enrollment_date, gpa, email)
VALUES (1, 'John', 'Doe', '2000-01-01', '2023-08-15', 3.8, 'john.doe@example.com');
```

Inserting multiple rows.
```sql
INSERT INTO students (student_id, first_name, last_name, date_of_birth, enrollment_date, gpa, email)
VALUES 
(2, 'Jane', 'Smith', '1999-12-12', '2023-08-15', 3.6, 'jane.smith@example.com'),
(3, 'Alice', 'Johnson', '2001-05-21', '2023-08-15', 3.9, 'alice.johnson@example.com');
```

### 3. UPDATE
Used to modify existing rows in a table.

#### Syntax
```sql
UPDATE table_name
SET column1 = value1, column2 = value2, ...
WHERE condition;
```

#### Example
Updating the GPA of a student.
```sql
UPDATE students
SET gpa = 3.9
WHERE student_id = 1;
```

Updating multiple columns.
```sql
UPDATE students
SET gpa = 4.0, email = 'new.email@example.com'
WHERE student_id = 1;
```

### 4. DELETE
Used to remove rows from a table.

#### Syntax
```sql
DELETE FROM table_name
WHERE condition;
```

#### Example
Deleting a student by `student_id`.
```sql
DELETE FROM students
WHERE student_id = 1;
```

Deleting all students with a GPA less than 2.0.
```sql
DELETE FROM students
WHERE gpa < 2.0;
```

### Comprehensive Example

Let's create the `students` table and perform some DML operations.

#### Creating the `students` Table
```sql
CREATE TABLE students (
    student_id INT PRIMARY KEY,
    first_name VARCHAR(50) NOT NULL,
    last_name VARCHAR(50) NOT NULL,
    date_of_birth DATE,
    enrollment_date DATE,
    gpa DECIMAL(3, 2) CHECK (gpa >= 0.0 AND gpa <= 4.0),
    email VARCHAR(100) UNIQUE
);
```

#### Inserting Data
```sql
INSERT INTO students (student_id, first_name, last_name, date_of_birth, enrollment_date, gpa, email)
VALUES 
(1, 'John', 'Doe', '2000-01-01', '2023-08-15', 3.8, 'john.doe@example.com'),
(2, 'Jane', 'Smith', '1999-12-12', '2023-08-15', 3.6, 'jane.smith@example.com'),
(3, 'Alice', 'Johnson', '2001-05-21', '2023-08-15', 3.9, 'alice.johnson@example.com');
```

#### Querying Data
```sql
SELECT * FROM students;
```

#### Updating Data
```sql
UPDATE students
SET gpa = 3.9
WHERE student_id = 1;
```

#### Deleting Data
```sql
DELETE FROM students
WHERE student_id = 2;
```

These examples cover the basic operations of data manipulation in SQL using a `students` table.