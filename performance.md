
# SQL Performance & Optimization Roadmap

## Objective
Learn how to analyze, optimize, and scale SQL queries and database systems.

Correct query ≠ Fast query.  
Performance is about minimizing work.

---

# 1️⃣ How Databases Execute Queries

## Learn

- What is a Query Planner?
- What is a Query Plan?
- Sequential Scan vs Index Scan
- Cost estimation basics

Understand:
The database decides how to execute your query.
Your job is to guide it correctly.

## Practice

- Use EXPLAIN
- Use EXPLAIN ANALYZE (PostgreSQL)

## Free Resources

- PostgreSQL EXPLAIN  
  https://www.postgresql.org/docs/current/using-explain.html

- Use The Index, Luke (Query Plans)  
  https://use-the-index-luke.com/sql/explain-plan

---

# 2️⃣ Indexing (Deep Dive)

## Learn

- What is a B-Tree index?
- When to add indexes
- Single vs Composite indexes
- Index on WHERE columns
- Index on JOIN columns
- Trade-offs (writes become slower)

Understand:
Indexes reduce search time.
But too many indexes hurt performance.

## Practice

- Compare query with and without index
- Create composite index
- Drop unnecessary indexes

## Free Resources

- PostgreSQL Indexes  
  https://www.postgresql.org/docs/current/indexes.html

- Use The Index, Luke  
  https://use-the-index-luke.com/

---

# 3️⃣ Query Optimization Techniques

## Learn

- Avoid SELECT *
- Use proper WHERE filtering
- Reduce subqueries when possible
- Use JOIN instead of correlated subquery (when needed)
- Proper use of LIMIT

Understand:
Less data scanned = faster queries.

## Practice

- Rewrite slow queries
- Compare execution plans
- Optimize JOIN-heavy queries

## Resource

- Mode SQL Performance Guide  
  https://mode.com/sql-tutorial/sql-performance-tuning/

---

# 4️⃣ Transactions & Concurrency

## Learn

- What is concurrency?
- Locks (Row-level, Table-level)
- Deadlocks
- Isolation levels:
  - Read Uncommitted
  - Read Committed
  - Repeatable Read
  - Serializable

Understand:
Concurrency problems happen in real systems, not tutorials.

## Free Resources

- PostgreSQL Transaction Isolation  
  https://www.postgresql.org/docs/current/transaction-iso.html

- PostgreSQL Explicit Locking  
  https://www.postgresql.org/docs/current/explicit-locking.html

---

# 5️⃣ Query Anti-Patterns

Avoid:

- Functions in WHERE clause (kills index usage)
- Leading wildcard in LIKE ('%text')
- Missing indexes on JOIN columns
- Huge OFFSET pagination
- Unnecessary DISTINCT

Understand:
Small design mistakes create exponential slowdown.

## Resource

- Use The Index, Luke Anti-Patterns  
  https://use-the-index-luke.com/sql/where-clause

---

# 6️⃣ Scaling Concepts (Advanced Awareness)

## Learn

- Partitioning
- Replication (Read replicas)
- Connection pooling
- Caching (Redis overview)
- Sharding (conceptual level)

Understand:
Scaling is architectural, not just query-level.

## Free Resources

- PostgreSQL Partitioning  
  https://www.postgresql.org/docs/current/ddl-partitioning.html

- DigitalOcean Scaling Guide  
  https://www.digitalocean.com/community/tutorials/an-introduction-to-sql-performance-tuning

---

# 7️⃣ Performance Testing Practice

## Practice Tasks

- Insert 100k+ rows
- Benchmark queries before and after indexing
- Compare execution plans
- Create slow query intentionally and fix it

---

# Tools to Use

- PostgreSQL
- pgAdmin
- DBeaver
- EXPLAIN ANALYZE

---

# Mastery Checklist

- [ ] I understand query plans
- [ ] I know when to add indexes
- [ ] I can optimize JOIN-heavy queries
- [ ] I understand lock behavior
- [ ] I can explain isolation levels
- [ ] I benchmarked real queries

---

# Deliverable

Inside this folder create:

- slow_queries.sql
- optimized_queries.sql
- indexing_tests.sql
- explain_analysis.sql

Run performance comparisons and document findings.
