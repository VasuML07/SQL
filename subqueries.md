# SQL Subqueries & CTE Roadmap

## Objective
Master nested queries, correlated logic, and Common Table Expressions (CTEs).

Subqueries allow SQL to think in layers.  
CTEs allow SQL to think clearly.

---

# 1️⃣ What is a Subquery?

## Learn

- What is a subquery?
- Where subqueries can be used:
  - SELECT
  - WHERE
  - FROM
- Scalar subquery (returns one value)
- Subquery returning multiple rows

Understand:
A subquery is a query inside another query.
It executes before the outer query (in most cases).

## Practice

- Get employees earning above average salary
- Find products priced above category average
- Filter users with more than 5 orders

## Free Resources

- W3Schools Subquery  
  https://www.w3schools.com/sql/sql_subqueries.asp

- SQLBolt Subqueries  
  https://sqlbolt.com/lesson/select_queries_with_subqueries

- Mode SQL Subqueries  
  https://mode.com/sql-tutorial/sql-subqueries/

---

# 2️⃣ Correlated Subqueries (Important)

## Learn

- What makes a subquery correlated
- How it references outer query
- Performance implications

Understand:
Correlated subqueries run once per row of outer query.
They can be expensive.

Example idea:
Compare each employee salary to department average.

## Practice

- Find customers who placed more orders than average
- Compare each product price to overall average

## Resource

- Mode Correlated Subqueries  
  https://mode.com/sql-tutorial/sql-correlated-subqueries/

---

# 3️⃣ EXISTS vs IN

## Learn

- EXISTS
- IN
- NOT EXISTS
- NOT IN
- Performance differences

Understand:
EXISTS checks if rows exist.
IN compares against a set of values.

Important:
NOT IN behaves differently with NULL values.

## Practice

- Customers who have orders
- Customers who never ordered

## Resource

- PostgreSQL Subquery Expressions  
  https://www.postgresql.org/docs/current/functions-subquery.html

---

# 4️⃣ Subqueries in FROM (Derived Tables)

## Learn

- Subquery inside FROM
- Aliasing derived tables
- Aggregating then filtering

Understand:
Derived tables create temporary result sets.

## Practice

- Calculate average revenue per user, then filter
- Rank products by category sales

---

# 5️⃣ Common Table Expressions (CTE)

## Learn

- WITH clause
- Writing readable layered queries
- Multiple CTEs
- Recursive CTE (basic idea)

Understand:
CTE improves readability.
It does not always improve performance.

## Practice

- Rewrite complex subquery using CTE
- Chain multiple CTE blocks
- Hierarchy example (employee-manager)

## Free Resources

- PostgreSQL WITH Queries  
  https://www.postgresql.org/docs/current/queries-with.html

- Mode CTE Guide  
  https://mode.com/sql-tutorial/sql-common-table-expressions/

---

# 6️⃣ Window Functions (Advanced Layer)

## Learn

- OVER()
- PARTITION BY
- ORDER BY inside window
- ROW_NUMBER()
- RANK()
- DENSE_RANK()
- LAG()
- LEAD()

Understand:
Window functions do not collapse rows.
They compute values across a set of rows.

This is advanced analytical SQL.

## Practice

- Top 3 salaries per department
- Running totals
- Ranking products per category

## Free Resources

- PostgreSQL Window Functions  
  https://www.postgresql.org/docs/current/tutorial-window.html

- Mode Window Functions  
  https://mode.com/sql-tutorial/sql-window-functions/

---

# 7️⃣ Performance Awareness

## Learn

- When subqueries hurt performance
- Rewriting correlated subquery into JOIN
- CTE materialization (PostgreSQL behavior)

Understand:
Readability and performance are not always aligned.

## Resource

- Use The Index, Luke – Subqueries  
  https://use-the-index-luke.com/sql/subquery

---

# Practice Platforms

Focus on advanced SQL questions:

- LeetCode SQL  
  https://leetcode.com/problemset/database/

- HackerRank Advanced SQL  
  https://www.hackerrank.com/domains/sql

- SQLZoo Advanced  
  https://sqlzoo.net/wiki/Advanced_SELECT

---

# Mastery Checklist

- [ ] I understand scalar vs multi-row subqueries
- [ ] I can write correlated subqueries confidently
- [ ] I know difference between EXISTS and IN
- [ ] I can rewrite subqueries as CTE
- [ ] I understand window functions
- [ ] I solved 60+ advanced SQL problems

---

# Deliverable

Inside this folder create:

- subqueries.sql
- correlated_subqueries.sql
- cte_examples.sql
- window_functions.sql

Write at least:
- 20 subquery problems
- 10 CTE-based queries
- 10 window function queries
