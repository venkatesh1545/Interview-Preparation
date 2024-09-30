# DBMS Interview Questions and Answers

### Table of Contents
1. [What is a Database?](#what-is-a-database)
2. [What is DBMS (Database Management System)?](#what-is-dbms)
3. [What is the difference between a DBMS and an RDBMS?](#what-is-the-difference-between-a-dbms-and-an-rdbms)
4. [What are ACID properties?](#what-are-acid-properties)
5. [What is Normalization? Why is it important?](#what-is-normalization-why-is-it-important)
6. [What is Denormalization? When would you use it?](#what-is-denormalization-when-would-you-use-it)
7. [What are the different types of Normalization?](#what-are-the-different-types-of-normalization)
8. [What is a primary key?](#what-is-a-primary-key)
9. [What is a foreign key?](#what-is-a-foreign-key)
10. [What are indexes in a database?](#what-are-indexes-in-a-database)
11. [What are the different types of indexes?](#what-are-the-different-types-of-indexes)
12. [What is a View?](#what-is-a-view)
13. [What is a JOIN in SQL?](#what-is-a-join-in-sql)
14. [What is a Transaction?](#what-is-a-transaction)
15. [What is Referential Integrity?](#what-is-referential-integrity)
16. [What are Triggers in a database?](#what-are-triggers-in-a-database)
17. [What are Stored Procedures?](#what-are-stored-procedures)
18. [What is the difference between DELETE, TRUNCATE, and DROP?](#what-is-the-difference-between-delete-truncate-and-drop)
19. [What are Constraints in SQL?](#what-are-constraints-in-sql)
20. [What is the difference between UNION and UNION ALL?](#what-is-the-difference-between-union-and-union-all)
21. [What is the difference between a clustered and a non-clustered index?](#what-is-the-difference-between-a-clustered-and-a-non-clustered-index)
22. [Explain the concept of a deadlock in DBMS. How can it be avoided?](#explain-the-concept-of-a-deadlock-in-dbms-how-can-it-be-avoided)
23. [What is a surrogate key in DBMS?](#what-is-a-surrogate-key-in-dbms)

---

### Answers

#### What is a Database?
A database is a structured collection of data that is stored and managed electronically. It is designed to efficiently store, retrieve, and manipulate data. Databases are essential for managing large amounts of structured information.

#### What is DBMS?
A Database Management System (DBMS) is software that interacts with users, applications, and the database itself to capture and analyze data. The DBMS manages data, the database engine, and the database schema to facilitate the organization and manipulation of data.

#### What is the difference between a DBMS and an RDBMS?
A DBMS stores data as files, and it is mainly used for storing, modifying, and retrieving information. It doesn’t enforce relationships between tables.
An RDBMS (Relational Database Management System), on the other hand, stores data in a tabular form and ensures relationships between tables using foreign keys. RDBMS supports normalization and follows ACID properties (Atomicity, Consistency, Isolation, Durability).

#### What are ACID properties?
ACID properties ensure that database transactions are processed reliably:
- **Atomicity:** All operations within a transaction are completed; otherwise, the transaction is aborted.
- **Consistency:** The database must transition from one valid state to another valid state.
- **Isolation:** The operations of a transaction are invisible to other transactions until it is completed.
- **Durability:** Once a transaction is committed, it remains permanent, even in case of a system failure.

#### What is Normalization? Why is it important?
Normalization is the process of organizing data in a database to reduce redundancy and improve data integrity. It involves dividing a database into tables and defining relationships between the tables.

Benefits:
- Eliminates redundant data.
- Ensures data integrity and consistency.
- Optimizes queries by organizing the data structure.

#### What is Denormalization? When would you use it?
Denormalization is the process of adding redundancy to a database to improve read performance by reducing the number of joins required. This is useful in systems where performance is critical, such as OLAP (Online Analytical Processing) systems, or when frequent read operations outweigh the benefits of normalized tables.

#### What are the different types of Normalization?
Common Normalization forms include:
- **1NF (First Normal Form):** Ensures that the values in a table are atomic (indivisible).
- **2NF (Second Normal Form):** In addition to 1NF, ensures that all non-key attributes are fully dependent on the primary key.
- **3NF (Third Normal Form):** In addition to 2NF, ensures that no transitive dependency exists (i.e., non-key attributes should not depend on other non-key attributes).
- **BCNF (Boyce-Codd Normal Form):** A stricter version of 3NF where every determinant is a candidate key.

#### What is a primary key?
A primary key is a column (or a set of columns) that uniquely identifies each row in a table. A primary key ensures that there are no duplicate entries in the table, and the value in the primary key column cannot be NULL.

#### What is a foreign key?
A foreign key is a column (or a set of columns) that establishes a relationship between two tables. It refers to the primary key in another table, enforcing referential integrity between the two tables.

#### What are indexes in a database?
An index is a database object that improves the speed of data retrieval operations. Indexes are created on columns that are frequently queried. However, indexes also require additional storage and can slow down write operations like INSERT, UPDATE, and DELETE.

#### What are the different types of indexes?
- **Primary Index:** Created on the primary key of a table.
- **Unique Index:** Ensures that no two rows have the same value in the indexed column(s).
- **Clustered Index:** Reorders the actual table data to match the index. A table can have only one clustered index.
- **Non-clustered Index:** Does not alter the table’s order but creates a separate structure for fast lookups.

#### What is a View?
A view is a virtual table based on the result-set of an SQL query. Views do not store data themselves but retrieve it from one or more tables. They provide a way to simplify complex queries and control access to specific data.

#### What is a JOIN in SQL?
A JOIN is used to combine rows from two or more tables based on a related column between them. Types of joins include:
- **INNER JOIN:** Returns rows when there is a match in both tables.
- **LEFT JOIN:** Returns all rows from the left table and matched rows from the right table. If no match, returns NULL for right table columns.
- **RIGHT JOIN:** Returns all rows from the right table and matched rows from the left table.
- **FULL JOIN:** Returns rows when there is a match in one of the tables.
- **CROSS JOIN:** Returns the Cartesian product of the two tables.

#### What is a Transaction?
A transaction is a unit of work that contains a group of SQL operations. All operations within a transaction must either complete successfully or fail as a whole. Transactions are used to ensure data integrity and consistency.

#### What is Referential Integrity?
Referential integrity is a property that ensures relationships between tables remain consistent. Specifically, it ensures that a foreign key value always points to an existing row in the referenced table.

#### What are Triggers in a database?
A trigger is a database object that is automatically executed or fired when certain events occur, such as INSERT, UPDATE, or DELETE operations.

#### What are Stored Procedures?
A stored procedure is a precompiled collection of SQL statements that can be executed as a single unit.

#### What is the difference between DELETE, TRUNCATE, and DROP?
- **DELETE:** Removes specific rows from a table based on a condition. It is a DML operation and can be rolled back.
- **TRUNCATE:** Removes all rows from a table but keeps the structure intact. It is a DDL operation and cannot be rolled back.
- **DROP:** Deletes the entire table (or database), including its structure. It is also a DDL operation and is irreversible.

#### What are Constraints in SQL?
Constraints are rules applied to columns in a database to enforce data integrity. Types of constraints include:
- **NOT NULL**
- **UNIQUE**
- **PRIMARY KEY**
- **FOREIGN KEY**
- **CHECK**
- **DEFAULT**

#### What is the difference between UNION and UNION ALL?
- **UNION:** Combines the result sets of two queries and removes duplicate rows.
- **UNION ALL:** Combines the result sets of two queries but does not remove duplicates.

#### What is the difference between a clustered and a non-clustered index?
- **Clustered Index:** Alters the way records are stored in the database based on the key.
- **Non-clustered Index:** Creates a logical order for data rows and uses pointers to the actual physical data.

#### Explain the concept of a deadlock in DBMS. How can it be avoided?
A deadlock occurs when two or more transactions are waiting for each other to release locks on resources, leading to a situation where none of the transactions can proceed.

To avoid deadlocks:
- Use a consistent locking order.
- Implement a timeout mechanism.
- Use deadlock detection algorithms.

#### What is a surrogate key in DBMS?
A surrogate key is an artificial or synthetic key used as a unique identifier for a table. It is often a sequential number and has no inherent meaning outside the database.

---

