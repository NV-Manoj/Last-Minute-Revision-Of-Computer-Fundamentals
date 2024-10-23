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
10. [ACID Properties](#acid-properties)
11. [Database Security](#database-security)
12. [Important SQL Queries](#important-sql-queries)

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

5. **Join Query**:
   ```sql
   SELECT column_name(s) FROM table1
   INNER JOIN table2 ON table1.column = table2.column;
   ```

---

### **Pro-Tip**:
- Be clear about **query optimization** and **execution plans**.
- Understand **ER Diagrams** (Entity-Relationship Diagrams).
- Practice common SQL problems like subqueries, aggregate functions (`COUNT()`, `SUM()`, `GROUP BY`), and set operations (`UNION`, `INTERSECT`).

---

Good luck with your interview preparation! 🚀

---

