# SQL Joins Roadmap

## Objective
Master how to combine data from multiple tables using relational logic.

Joins are controlled row matching.
If you understand relationships, joins become predictable.

---

# 1️⃣ Why Joins Exist

## Learn

- Why relational databases split data into multiple tables
- Primary key vs Foreign key recap
- How relationships map to joins

Understand:
A join matches rows based on a condition (usually keys).

Example mental model:
Users table + Orders table  
Match where users.id = orders.user_id

## Free Resources

- Khan Academy Relational Queries  
  https://www.khanacademy.org/computing/computer-programming/sql

- SQLBolt Join Lesson  
  https://sqlbolt.com/lesson/select_queries_with_joins

---

# 2️⃣ INNER JOIN (Foundation)

## Learn

- INNER JOIN syntax
- ON condition
- What happens when no match exists
- Table aliases

Understand:
INNER JOIN returns only matching rows.

## Practice

- Users with their orders
- Students with their courses
- Employees with departments

## Free Resources

- W3Schools INNER JOIN  
  https://www.w3schools.com/sql/sql_join_inner.asp

- Mode SQL Tutorial – Joins  
  https://mode.com/sql-tutorial/sql-joins/

---

# 3️⃣ LEFT JOIN (Critical Skill)

## Learn

- LEFT JOIN behavior
- NULL values in unmatched rows
- When LEFT JOIN is necessary

Understand:
LEFT JOIN keeps all rows from left table.
Missing matches become NULL.

## Practice

- Customers who never ordered
- Products with no sales
- Users without profiles

## Free Resources

- W3Schools LEFT JOIN  
  https://www.w3schools.com/sql/sql_join_left.asp

---

# 4️⃣ RIGHT JOIN & FULL JOIN

## Learn

- RIGHT JOIN
- FULL OUTER JOIN
- When they are useful
- Why many systems rarely use RIGHT JOIN

Understand:
FULL JOIN returns all rows from both tables.

## Free Resources

- W3Schools FULL JOIN  
  https://www.w3schools.com/sql/sql_join_full.asp

- PostgreSQL Join Types  
  https://www.postgresql.org/docs/current/tutorial-join.html

---

# 5️⃣ Multiple Joins (3+ Tables)

## Learn

- Joining more than two tables
- Join order
- Readability using aliases

Understand:
Join complexity grows quickly.
Clarity matters.

## Practice

Ecommerce example:
Customers → Orders → Order_Items → Products

---

# 6️⃣ Self Joins

## Learn

- Joining a table to itself
- Use cases:
  - Employee-manager hierarchy
  - Referral systems
  - Category trees

## Practice

- Employees and their managers
- Find duplicate relationships

## Resource

- SQLZoo Self Join  
  https://sqlzoo.net/wiki/Self_join

---

# 7️⃣ Join + Aggregation

## Learn

- GROUP BY with JOIN
- Aggregating after combining tables
- Order of execution

Understand:
JOIN happens before GROUP BY.

## Practice

- Total spending per customer
- Average salary per department
- Orders per product category

---

# 8️⃣ Common Join Mistakes

Avoid:

- Forgetting ON condition
- Joining on wrong columns
- Cartesian product (accidental cross join)
- Filtering in wrong place (WHERE vs ON)

Understand:
Missing ON condition = explosion of rows.

---

# Practice Platforms

Solve at least 60–80 join problems.

- LeetCode SQL  
  https://leetcode.com/problemset/database/

- HackerRank SQL  
  https://www.hackerrank.com/domains/sql

- SQLZoo Join Exercises  
  https://sqlzoo.net/wiki/More_JOIN_operations

---

# Mastery Checklist

- [ ] I understand INNER JOIN completely
- [ ] I can explain LEFT JOIN without confusion
- [ ] I can join 3+ tables confidently
- [ ] I can detect cartesian products
- [ ] I solved 70+ join problems
- [ ] I built a 5-table relational system

---

# Deliverable

Create inside this folder:

- ecommerce_schema.sql
- join_practice.sql
- advanced_joins.sql

Build a system with at least:
- 5 tables
- Proper foreign keys
- 20+ join queries
