
# Database Design Roadmap

## Objective
Learn how to design scalable, clean, and efficient relational databases.

Good schema = long-term stability.  
Bad schema = permanent technical debt.

---

# 1️⃣ Relational Thinking

## Learn

- What is the relational model?
- Entities vs Attributes
- One-to-One relationships
- One-to-Many relationships
- Many-to-Many relationships
- Junction (bridge) tables

Understand:
Tables represent real-world entities.  
Relationships define how they connect.

## Free Resources

- Khan Academy Relational Databases  
  https://www.khanacademy.org/computing/computer-programming/sql

- Lucidchart ER Diagram Guide  
  https://www.lucidchart.com/pages/er-diagrams

---

# 2️⃣ Primary Keys & Foreign Keys

## Learn

- PRIMARY KEY
- FOREIGN KEY
- Composite keys
- Surrogate vs Natural keys
- ON DELETE CASCADE
- ON UPDATE CASCADE

Understand:
Primary key = identity  
Foreign key = relationship enforcement  

## Free Resources

- PostgreSQL Constraints  
  https://www.postgresql.org/docs/current/ddl-constraints.html

- W3Schools SQL Constraints  
  https://www.w3schools.com/sql/sql_constraints.asp

---

# 3️⃣ Normalization (Critical Topic)

## Learn

- 1NF (Atomic columns)
- 2NF (No partial dependency)
- 3NF (No transitive dependency)
- Why denormalization exists

Understand:
Normalization reduces redundancy and prevents anomalies.

## Free Resources

- Normalization Explained Clearly  
  https://www.guru99.com/database-normalization.html

- Vertabelo Normalization Guide  
  https://www.vertabelo.com/blog/database-normalization/

---

# 4️⃣ Indexing (Performance Foundation)

## Learn

- What is an index?
- B-Tree concept (basic idea)
- When to use indexes
- Trade-offs of indexing
- Composite indexes

Understand:
Indexes speed up reads but slow down writes.

## Free Resources

- PostgreSQL Indexes  
  https://www.postgresql.org/docs/current/indexes.html

- Use The Index, Luke  
  https://use-the-index-luke.com/

---

# 5️⃣ Constraints & Data Integrity

## Learn

- NOT NULL
- UNIQUE
- CHECK
- DEFAULT
- Referential integrity

Understand:
Constraints protect your data from bad inserts.

## Free Resources

- PostgreSQL Constraints  
  https://www.postgresql.org/docs/current/ddl-constraints.html

---

# 6️⃣ Transactions & ACID

## Learn

- What is a transaction?
- COMMIT
- ROLLBACK
- ACID properties:
  - Atomicity
  - Consistency
  - Isolation
  - Durability

Understand:
Transactions guarantee reliability in concurrent systems.

## Free Resources

- PostgreSQL Transactions  
  https://www.postgresql.org/docs/current/tutorial-transactions.html

- ACID Explained (Simple)  
  https://www.geeksforgeeks.org/acid-properties-in-dbms/

---

# 7️⃣ Schema Design Practice

## Practice Systems

Design databases for:

- E-commerce system
- School management system
- Social media platform
- Hospital system

For each:
- Draw ER diagram
- Normalize to 3NF
- Define constraints
- Add indexes

---

# 8️⃣ Common Design Mistakes

Avoid:

- Storing comma-separated values in one column
- Missing foreign keys
- Overusing TEXT fields
- No indexing on frequent filters
- No unique constraints on critical fields

---

# Practice Platforms

- DrawSQL (Free ER Diagram Tool)  
  https://drawsql.app/

- dbdiagram.io  
  https://dbdiagram.io/

- LeetCode SQL (Schema-based questions)  
  https://leetcode.com/problemset/database/

---

# Mastery Checklist

- [ ] I understand entity relationships clearly
- [ ] I can design a schema from scratch
- [ ] I can normalize tables to 3NF
- [ ] I know when to add indexes
- [ ] I understand ACID properties
- [ ] I designed at least 3 full systems

---

# Deliverable

Inside this folder create:

- ecommerce_schema.sql
- school_schema.sql
- social_media_schema.sql
- normalization_examples.md

Each schema must:
- Use primary keys
- Use foreign keys
- Include constraints
- Include indexes
