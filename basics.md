# SQL Basics Roadmap

## Objective
Build strong foundations in querying and manipulating relational databases.

Master syntax. Understand execution order. Avoid guessing.

---

# 1️⃣ Understanding Databases

## Learn

- What is a database?
- What is a table?
- Row vs Column
- Primary Key
- Foreign Key (basic idea)
- Relational model basics

Understand:
Tables represent entities.  
Rows represent instances.  
Columns represent attributes.

## Free Resources

- PostgreSQL Official Tutorial  
  https://www.postgresql.org/docs/current/tutorial-start.html

- Khan Academy Intro to SQL  
  https://www.khanacademy.org/computing/computer-programming/sql

---

# 2️⃣ SELECT Statement (Core Skill)

## Learn

- SELECT *
- SELECT specific columns
- Column aliases (AS)
- DISTINCT

## Practice

- Select all records
- Select specific columns
- Remove duplicates

## Free Resources

- SQLBolt Lessons 1–4  
  https://sqlbolt.com/

- W3Schools SELECT  
  https://www.w3schools.com/sql/sql_select.asp

---

# 3️⃣ Filtering Data (WHERE Clause)

## Learn

- WHERE
- Comparison operators (=, >, <, >=, <=)
- AND / OR / NOT
- BETWEEN
- IN
- LIKE
- IS NULL / IS NOT NULL

Understand:
Filtering happens before grouping.

## Practice

- Filter users by age
- Find orders within date range
- Find names starting with "A"
- Filter NULL values

## Free Resources

- SQLBolt Filtering  
  https://sqlbolt.com/lesson/filtering_rows

- Mode SQL Tutorial (Filtering)  
  https://mode.com/sql-tutorial/sql-where/

---

# 4️⃣ Sorting & Limiting

## Learn

- ORDER BY
- ASC / DESC
- LIMIT
- OFFSET

## Practice

- Get top 5 highest salaries
- Get latest 10 orders

## Free Resources

- W3Schools ORDER BY  
  https://www.w3schools.com/sql/sql_orderby.asp

- SQLBolt Sorting  
  https://sqlbolt.com/lesson/sorting_results

---

# 5️⃣ Inserting Data

## Learn

- INSERT INTO
- Insert single row
- Insert multiple rows

## Practice

- Insert users
- Insert product records

## Free Resources

- W3Schools INSERT  
  https://www.w3schools.com/sql/sql_insert.asp

---

# 6️⃣ Updating & Deleting Data

## Learn

- UPDATE
- DELETE
- Importance of WHERE
- Safe updates

Understand:
Forgetting WHERE = disaster.

## Practice

- Update salary of one employee
- Delete specific records

## Free Resources

- W3Schools UPDATE  
  https://www.w3schools.com/sql/sql_update.asp

- W3Schools DELETE  
  https://www.w3schools.com/sql/sql_delete.asp

---

# 7️⃣ Creating Tables (DDL Basics)

## Learn

- CREATE TABLE
- Data types (INT, VARCHAR, DATE, BOOLEAN)
- PRIMARY KEY
- NOT NULL
- UNIQUE

Basic schema design.

## Free Resources

- PostgreSQL Data Types  
  https://www.postgresql.org/docs/current/datatype.html

- W3Schools CREATE TABLE  
  https://www.w3schools.com/sql/sql_create_table.asp

---

# 8️⃣ Execution Order (Critical Concept)

Understand how SQL actually runs:

1. FROM
2. WHERE
3. SELECT
4. ORDER BY
5. LIMIT

This prevents logical mistakes later.

## Resource

- Mode SQL Execution Order  
  https://mode.com/sql-tutorial/sql-order-of-operations/

---

# Practice Platforms

Solve at least 40–60 basic problems.

- LeetCode SQL  
  https://leetcode.com/problemset/database/

- HackerRank SQL  
  https://www.hackerrank.com/domains/sql

- SQLZoo  
  https://sqlzoo.net/

---

# Mastery Checklist

- [ ] I can write SELECT without looking up syntax
- [ ] I understand WHERE logic operators
- [ ] I know how NULL behaves
- [ ] I can sort and limit results
- [ ] I can safely UPDATE and DELETE
- [ ] I created at least 3 tables manually
- [ ] I solved 50+ beginner SQL problems

---

# Deliverable

Create:

- schema.sql
- insert_data.sql
- queries.sql

Build a small dataset (students, ecommerce, or library system)  
and write 20–30 queries covering everything above.
