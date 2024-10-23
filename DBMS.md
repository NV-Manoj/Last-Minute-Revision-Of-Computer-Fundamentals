# LastMinuteRevision

Here's a concise last-minute revision guide for **DBMS (Database Management System)**, formatted as a **README.md** file to help prepare for interviews.

---

# Last-Minute Revision Notes for DBMS

## Table of Contents
1. [Basic Concepts](#basic-concepts)
2. [Database Models](#database-models)
3. [Normalization](#normalization)
4. [SQL](#sql)
5. [Transactions](#transactions)
6. [Concurrency Control](#concurrency-control)
7. [Indexing](#indexing)
8. [Keys](#keys)
9. [Joins](#joins)
10. [Views](#Views)
11. [Procedures](#Procedures)
12. [ACID Properties](#acid-properties)
13. [Database Security](#database-security)
14. [Important SQL Queries](#important-sql-queries)
15. [Triggers (Optional)](#Triggers)
---

## 1. Basic Concepts

- **DBMS**: A software that handles the storage, retrieval, and updating of data in a database.
- **Database**: An organized collection of data.
- **Schema**: Structure of a database (tables, columns, etc.).
- **Instance**: Snapshot of the data in a database at a particular moment.

## 2. Database Models

- **Hierarchical Model**: Tree-like structure; parent-child relationship.
- **Network Model**: More complex, graph-like structure, allowing many-to-many relationships.
- **Relational Model**: Data is stored in tables (relations). The most commonly used model.
- **Object-Oriented Model**: Data is stored as objects, similar to OOP concepts.

## 3. Normalization

- **1NF (First Normal Form)**: Eliminate duplicate columns and create separate tables for related data.
- **2NF (Second Normal Form)**: Eliminate partial dependency (no non-prime attribute should depend on part of a candidate key).
- **3NF (Third Normal Form)**: Eliminate transitive dependency (no non-prime attribute should depend on another non-prime attribute).
- **BCNF (Boyce-Codd Normal Form)**: Every determinant must be a candidate key.
  
## 4. SQL

- **DDL (Data Definition Language)**: Defines the schema. Includes `CREATE`, `ALTER`, `DROP`, `TRUNCATE`.
- **DML (Data Manipulation Language)**: Deals with data manipulation. Includes `SELECT`, `INSERT`, `UPDATE`, `DELETE`.
- **DCL (Data Control Language)**: Deals with permissions. Includes `GRANT`, `REVOKE`.
- **TCL (Transaction Control Language)**: Controls transactions. Includes `COMMIT`, `ROLLBACK`, `SAVEPOINT`.

## 5. Transactions

- **Transaction**: A sequence of operations performed as a single logical unit of work.
- **States**:
  - **Active**: Transaction is being executed.
  - **Partially Committed**: All operations are completed but not yet committed.
  - **Committed**: Transaction is successfully executed and saved to the database.
  - **Failed**: Execution stopped due to a failure.
  - **Aborted**: Transaction is rolled back.
  
## 6. Concurrency Control

- **Locks**: Mechanism to control access to data. Types:
  - **Shared Lock**: Allows multiple transactions to read data.
  - **Exclusive Lock**: Only one transaction can modify data.
- **Deadlock**: A situation where two or more transactions are waiting for each other to release locks.
- **Solutions to Deadlocks**: Timeout, Wait-Die, Wound-Wait, Deadlock Detection.

## 7. Indexing

- **Index**: A data structure that improves the speed of data retrieval operations.
- **Types of Indexes**:
  - **Primary Index**: Created on the primary key.
  - **Secondary Index**: Created on non-primary key attributes.
  - **Clustered Index**: Alters the physical order of the table.
  - **Non-Clustered Index**: Does not alter the physical order.

## 8. Keys

- **Primary Key**: Uniquely identifies each record in a table.
- **Foreign Key**: Ensures referential integrity between two tables.
- **Candidate Key**: A minimal superkey, which can be a primary key.
- **Composite Key**: A key consisting of two or more attributes.
- **Superkey**: A set of attributes that uniquely identifies a row.

## 9. Joins

- **Inner Join**: Returns records with matching values in both tables.
- **Left Join**: Returns all records from the left table, and matched records from the right.
- **Right Join**: Returns all records from the right table, and matched records from the left.
- **Full Join**: Returns all records when there is a match in either table.
- **Cross Join**: Returns the Cartesian product of the two tables.

## 10. ACID Properties

- **Atomicity**: Ensures that a transaction is either fully completed or not at all.
- **Consistency**: Ensures the database is in a valid state before and after a transaction.
- **Isolation**: Ensures that transactions are executed independently.
- **Durability**: Ensures that once a transaction is committed, it remains permanent.

## 11. Database Security

- **Authentication**: Verifies the identity of users.
- **Authorization**: Determines what an authenticated user is allowed to do.
- **Encryption**: Converts data into a secure format to prevent unauthorized access.
- **Backup and Recovery**: Ensures data can be restored in case of failure.

## 12. Important SQL Queries

1. **Select Query**:
   ```sql
   SELECT * FROM table_name WHERE condition;
   ```

2. **Insert Query**:
   ```sql
   INSERT INTO table_name (column1, column2) VALUES (value1, value2);
   ```

3. **Update Query**:
   ```sql
   UPDATE table_name SET column1 = value1 WHERE condition;
   ```

4. **Delete Query**:
   ```sql
   DELETE FROM table_name WHERE condition;
   ```

Here’s an extended section starting with **Joins**, followed by **Views** and **Procedures** in a structured format for your revision:

---

## 9. Joins

Joins are used to combine rows from two or more tables based on a related column.

### Types of Joins:

1. **Inner Join**:
   - Returns only the rows where there is a match in both tables.
   ```sql
   SELECT column_name(s)
   FROM table1
   INNER JOIN table2
   ON table1.column = table2.column;
   ```

2. **Left (Outer) Join**:
   - Returns all rows from the left table and the matched rows from the right table. Unmatched rows from the right table will be NULL.
   ```sql
   SELECT column_name(s)
   FROM table1
   LEFT JOIN table2
   ON table1.column = table2.column;
   ```

3. **Right (Outer) Join**:
   - Returns all rows from the right table and the matched rows from the left table. Unmatched rows from the left table will be NULL.
   ```sql
   SELECT column_name(s)
   FROM table1
   RIGHT JOIN table2
   ON table1.column = table2.column;
   ```

4. **Full (Outer) Join**:
   - Returns all rows when there is a match in either table. Unmatched rows in both tables will show NULL.
   ```sql
   SELECT column_name(s)
   FROM table1
   FULL OUTER JOIN table2
   ON table1.column = table2.column;
   ```

5. **Cross Join**:
   - Returns the Cartesian product of the two tables, i.e., all combinations of rows.
   ```sql
   SELECT column_name(s)
   FROM table1
   CROSS JOIN table2;
   ```

6. **Self Join**:
   - Joins a table with itself.
   ```sql
   SELECT a.column_name, b.column_name
   FROM table_name a, table_name b
   WHERE condition;
   ```

---

## 10. Views

### Definition:
A **View** is a virtual table based on the result of a `SELECT` query. It doesn’t store data itself, but presents data from one or more tables.

### Creating a View:
```sql
CREATE VIEW view_name AS
SELECT column1, column2, ...
FROM table_name
WHERE condition;
```

### Using a View:
You can use a view just like a regular table in `SELECT`, `INSERT`, `UPDATE`, and `DELETE` operations (with some limitations).

```sql
SELECT * FROM view_name;
```

### Dropping a View:
```sql
DROP VIEW view_name;
```

---

## 11. Procedures

### Definition:
A **Stored Procedure** is a prepared SQL code that you can save and reuse. It is a set of SQL statements that perform a specific task.

### Creating a Procedure:
```sql
CREATE PROCEDURE procedure_name (parameter1 datatype, parameter2 datatype, ...)
BEGIN
   -- SQL statements here
   SELECT column_name FROM table_name WHERE condition;
END;
```

### Example of a Simple Procedure:
```sql
CREATE PROCEDURE GetEmployeeSalary (IN emp_id INT)
BEGIN
   SELECT salary
   FROM employees
   WHERE employee_id = emp_id;
END;
```

### Executing a Procedure:
```sql
CALL procedure_name (parameter1, parameter2, ...);
```

### Dropping a Procedure:
```sql
DROP PROCEDURE procedure_name;
```

### Handling Parameters:
- **IN**: Input parameter (passed into the procedure).
- **OUT**: Output parameter (returned from the procedure).
- **INOUT**: Both input and output parameter.

---
## 12. Triggers
**Triggers** are not mandatory in a database, but they can be very useful depending on the situation. Let’s break down the use and importance of triggers in the context of databases:

## What are Triggers?

A **Trigger** is a database object that is automatically executed or fired when certain events occur in the database. It can be set to trigger on actions like `INSERT`, `UPDATE`, or `DELETE` on a table.

### Syntax of a Trigger:

```sql
CREATE TRIGGER trigger_name
AFTER|BEFORE INSERT|UPDATE|DELETE
ON table_name
FOR EACH ROW
BEGIN
    -- SQL statements to execute
END;
```

### Example of a Trigger:

```sql
CREATE TRIGGER before_employee_update
BEFORE UPDATE
ON employees
FOR EACH ROW
BEGIN
   INSERT INTO audit_table(employee_id, old_salary, new_salary, update_time)
   VALUES (OLD.employee_id, OLD.salary, NEW.salary, NOW());
END;
```

In this example, the trigger runs **before** an update on the `employees` table and logs the changes in the `audit_table`.

---

## When are Triggers Useful?

- **Auditing**: Automatically log changes (inserts, updates, deletes) made to a table for security or record-keeping purposes.
- **Data Integrity**: Enforce complex business rules that can't easily be enforced with normal constraints (like foreign keys or check constraints).
- **Automation**: Automatically execute some actions based on database changes (e.g., updating related records).
- **Notifications**: Trigger events that notify other systems or users when critical data changes.

---

## Are Triggers Mandatory?

No, **triggers are not mandatory**. Whether to use them depends on your specific use case. Here are some considerations:

### **When to Use Triggers**:
1. **Auditing and Logging**: If you need to track every change made to a table for historical records.
2. **Complex Integrity Rules**: When enforcing rules that are hard to enforce using just constraints.
3. **Automating Workflows**: Automatically perform tasks, such as updating related data, sending notifications, or cascading changes.

### **When NOT to Use Triggers**:
1. **Performance**: Triggers can slow down the database performance if they are not used wisely (e.g., multiple triggers on frequently updated tables).
2. **Complexity**: Overusing triggers can make debugging or understanding data flows in your database more difficult.
3. **Better Alternatives**: Some tasks that triggers perform can be done more efficiently through application-level logic or by using stored procedures.

---

### Conclusion:

Triggers are **optional** but useful for certain situations where automation, auditing, or enforcing complex integrity rules is required. If your application can handle these cases efficiently without triggers (e.g., through application code or scheduled tasks), then triggers are not mandatory.



This structure helps you easily navigate through **Joins**, **Views**,**Procedures** and **Triggers** in SQL, which are often crucial in interviews. These examples will allow you to quickly write or explain SQL queries involving these key concepts.

---

### **Pro-Tip**:
- Be clear about **query optimization** and **execution plans**.
- Understand **ER Diagrams** (Entity-Relationship Diagrams).
- Practice common SQL problems like subqueries, aggregate functions (`COUNT()`, `SUM()`, `GROUP BY`), and set operations (`UNION`, `INTERSECT`).

---

Good luck with your interview preparation! 🚀

---

