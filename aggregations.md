# SQL Aggregations Roadmap

## Objective
Understand how to summarize, compress, and analyze data using aggregate functions.

---

# 1️⃣ Core Aggregate Functions

## Learn

- COUNT()
- SUM()
- AVG()
- MIN()
- MAX()

Understand:
- Difference between COUNT(*) and COUNT(column)
- How NULL affects aggregates
- Numeric vs non-numeric columns

## Practice

- Count total rows
- Calculate total revenue
- Find average salary
- Get highest/lowest values

## Free Resources

- W3Schools Aggregates  
  https://www.w3schools.com/sql/sql_count_avg_sum.asp

- SQLZoo Aggregate Tutorial  
  https://sqlzoo.net/wiki/SUM_and_COUNT

- Mode SQL Tutorial (Very Good)  
  https://mode.com/sql-tutorial/sql-aggregate-functions/

---

# 2️⃣ GROUP BY (Core Concept)

## Learn

- GROUP BY syntax
- Grouping by single column
- Grouping by multiple columns
- Aggregates with GROUP BY

Understand deeply:
GROUP BY turns rows into summarized buckets.

## Practice

- Total sales per category
- Average salary per department
- Orders per customer

## Free Resources

- W3Schools GROUP BY  
  https://www.w3schools.com/sql/sql_groupby.asp

- SQLBolt Lesson 11  
  https://sqlbolt.com/lesson/select_queries_with_aggregates

- PostgreSQL Official Docs (Clear + Precise)  
  https://www.postgresql.org/docs/current/tutorial-agg.html

---

# 3️⃣ HAVING (Filtering Groups)

## Learn

- Difference between WHERE and HAVING
- Using HAVING with aggregates
- Execution order of SQL query

Understand:
WHERE filters rows  
HAVING filters groups  

## Practice

- Customers with more than 5 orders
- Departments with avg salary > X
- Categories with total revenue > X

## Free Resources

- W3Schools HAVING  
  https://www.w3schools.com/sql/sql_having.asp

- SQLBolt Lesson 12  
  https://sqlbolt.com/lesson/select_queries_with_aggregates_pt_2

---

# 4️⃣ NULL Handling in Aggregations

## Learn

- How aggregates treat NULL
- COALESCE()
- COUNT(column) vs COUNT(*)

## Practice

- Replace NULL with 0
- Count only non-null entries

## Free Resources

- PostgreSQL COALESCE  
  https://www.postgresql.org/docs/current/functions-conditional.html

- Mode SQL Tutorial (NULL section)  
  https://mode.com/sql-tutorial/sql-null-values/

---

# 5️⃣ Advanced Aggregation Concepts

## Learn

- GROUP BY multiple columns
- Aggregate inside subqueries
- Conditional aggregation (CASE + SUM)

Example:
SUM(CASE WHEN status = 'paid' THEN amount ELSE 0 END)

## Practice

- Count paid vs unpaid orders
- Monthly revenue breakdown
- Customer segmentation

## Free Resources

- Mode SQL CASE  
  https://mode.com/sql-tutorial/sql-case/

- SQLZoo Advanced  
  https://sqlzoo.net/wiki/Using_GROUP_BY

---

# 6️⃣ Practice Platforms

Solve at least 40–60 problems focused only on aggregates.

- LeetCode SQL  
  https://leetcode.com/problemset/database/

- HackerRank SQL  
  https://www.hackerrank.com/domains/sql

- StrataScratch (Free Questions)  
  https://www.stratascratch.com/

---

# Mastery Checklist

- [ ] I understand COUNT vs COUNT(column)
- [ ] I can write GROUP BY without looking up syntax
- [ ] I can use HAVING correctly
- [ ] I understand NULL behavior
- [ ] I can write conditional aggregation
- [ ] I solved 50+ aggregation problems

---

# Deliverable

Create a mini dataset (ecommerce or school system) and write:

- Revenue per category
- Top 5 customers by spending
- Monthly order count
- Departments with salary > average salary

Commit it to:
02_aggregations/queries.sql
