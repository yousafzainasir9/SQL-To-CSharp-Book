# SQL to C# — The Complete Data Access Guide

**LINQ | Entity Framework | Dapper — Every concept explained from both sides**

> Most books explain data access from one perspective — either the database side or the OOP side. This book bridges the gap. Every concept starts as a relational database problem in raw SQL, then shows the exact C# equivalent in three ways: **LINQ Method Syntax**, **LINQ Query Syntax**, and **ORM-generated SQL**.

**[Read the Book Online](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/)**

---

## What Makes This Book Different

Traditional resources teach LINQ or Entity Framework in isolation. Developers coming from a SQL background struggle to map familiar concepts to OOP patterns — and OOP developers struggle to understand what their ORM is actually doing under the hood.

This book solves that by showing **every concept side-by-side**: the SQL way, the LINQ method chain way, and the LINQ query syntax way. You see the same operation through three lenses so the mental model clicks.

---

## Chapters

### Part 1 — The Two Worlds (Foundations)

| # | Chapter | Description |
|---|---------|-------------|
| 01 | [Tables vs Classes](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch01-tables-vs-classes.html) | How a database table maps to a C# class. Schema definition vs class properties. Column types vs CLR types. |
| 02 | [Rows vs Objects](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch02-rows-vs-objects.html) | A row is an instance. INSERT is construction. UPDATE is mutation. DELETE is disposal. CRUD through both lenses. |
| 03 | [Foreign Keys vs References](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch03-foreign-keys-vs-references.html) | How relational integrity maps to object references and navigation properties. Cascade rules vs object lifecycle. |
| 04 | [Relationships: Schema vs Object Graph](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch04-relationships.html) | One-to-One, One-to-Many, Many-to-Many — from junction tables and foreign keys to collections and navigation properties. |

### Part 2 — LINQ Fundamentals

| # | Chapter | Description |
|---|---------|-------------|
| 05 | [SELECT &rarr; .Select()](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch05-select-projections.html) | Projections in SQL vs LINQ. Column selection, aliases, computed columns, and anonymous types. |
| 06 | [WHERE &rarr; .Where()](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch06-where-filtering.html) | Filtering rows vs filtering objects. AND/OR logic, IN clauses, BETWEEN, NULL handling, and predicate translation. |
| 07 | [GROUP BY &rarr; .GroupBy()](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch07-groupby-aggregation.html) | Aggregation in SQL vs LINQ. COUNT, SUM, AVG, HAVING — and why LINQ's GroupBy returns something completely different. |
| 08 | [ORDER BY &rarr; .OrderBy()](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch08-orderby-sorting.html) | Sorting, multi-column ordering, ThenBy, custom comparers, and how sort operations affect query performance. |
| 09 | [JOINs &rarr; .Join() & Navigation](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch09-joins.html) | INNER, LEFT, CROSS joins in SQL vs LINQ's Join, GroupJoin, and EF's navigation-based approach. |
| 10 | [Subqueries &rarr; Nested LINQ](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch10-subqueries.html) | Correlated subqueries, EXISTS, IN with subquery, scalar subqueries — and their LINQ counterparts. |
| 11 | [Window Functions &rarr; LINQ Equivalents](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch11-window-functions.html) | ROW_NUMBER, RANK, LAG, LEAD, running totals — SQL features with no direct LINQ equivalent, and workarounds. |

### Part 3 — Entity Framework Core

| # | Chapter | Description |
|---|---------|-------------|
| 12 | [DbContext — Your Database in Code](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch12-dbcontext.html) | What DbContext represents. Connection management, DbSet as tables, OnModelCreating as schema definition. |
| 13 | [Migrations — Schema as Code](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch13-migrations.html) | ALTER TABLE vs Add-Migration. How EF tracks schema changes, generates SQL, and keeps database and code in sync. |
| 14 | [Loading Strategies](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch14-loading-strategies.html) | Eager, Lazy, and Explicit loading. What SQL each generates. Include() vs Select(), AsSplitQuery, and the N+1 problem. |
| 15 | [Change Tracking — How EF Thinks](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch15-change-tracking.html) | How EF detects changes, builds UPDATE statements, manages object state. AsNoTracking, ExecuteUpdate/ExecuteDelete. |
| 16 | [Raw SQL in EF Core](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch16-raw-sql-in-ef.html) | When the ORM isn't enough. FromSqlRaw, ExecuteSqlRaw, SQL interpolation, and mixing LINQ with raw SQL. |
| 17 | [EF Performance — N+1 and Beyond](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch17-ef-performance.html) | The N+1 problem visualized. AsNoTracking, split queries, compiled queries, batch operations, and reading EF-generated SQL. |

### Part 4 — Dapper (Micro-ORM)

| # | Chapter | Description |
|---|---------|-------------|
| 18 | [Connection & Queries](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch18-dapper-connection.html) | SqlConnection, Query&lt;T&gt;, Execute. How Dapper sits one step above raw ADO.NET and why that's powerful. |
| 19 | [Object Mapping](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch19-object-mapping.html) | How Dapper maps result sets to classes. Column-to-property matching, custom type handlers, multi-result-set mapping. |
| 20 | [Multi-Mapping Complex Joins](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch20-multi-mapping.html) | Mapping joined results into nested object graphs. splitOn explained, one-to-many patterns, and when to use multiple queries. |
| 21 | [Stored Procedures](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch21-stored-procedures.html) | Calling procs, passing parameters, handling output parameters and return values. When stored procedures beat inline SQL. |
| 22 | [Bulk Operations](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch22-bulk-operations.html) | INSERT 10,000 rows efficiently. SqlBulkCopy, table-valued parameters, Dapper Plus — compared to EF's SaveChanges. |

### Part 5 — Architecture Patterns

| # | Chapter | Description |
|---|---------|-------------|
| 23 | [Repository Pattern](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch23-repository-pattern.html) | Abstracting data access. Generic vs specific repositories. Repository with EF vs Dapper. When it helps vs pure indirection. |
| 24 | [Unit of Work](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch24-unit-of-work.html) | Transaction management across repositories. DbContext as built-in Unit of Work. UoW with Dapper and TransactionScope. |
| 25 | [CQRS — EF for Writes, Dapper for Reads](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch25-cqrs.html) | The pragmatic hybrid: EF's change tracking for commands, Dapper's speed for queries. Real implementation with MediatR. |
| 26 | [Choosing the Right Tool](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch26-choosing-the-right-tool.html) | Decision framework: when to use raw SQL, LINQ, EF Core, or Dapper. Benchmarks, trade-offs, and real-world scenarios. |

### Part 6 — Advanced Topics & Production Readiness

| # | Chapter | Description |
|---|---------|-------------|
| 27 | [Database Indexing](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch27-indexing.html) | B-Tree indexes, composite indexes, covering indexes. CREATE INDEX in SQL vs HasIndex() in EF. Reading execution plans. |
| 28 | [Transactions & Concurrency](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch28-transactions.html) | ACID properties, isolation levels, optimistic concurrency, deadlock prevention. SQL vs EF vs Dapper approaches. |
| 29 | [Testing Data Access Code](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch29-testing.html) | In-memory databases, SQLite for tests, TestContainers. Unit testing EF repositories and Dapper queries. |
| 30 | [SQL Injection Prevention](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch30-security.html) | How SQL injection works, parameterized queries as the fix. The dangerous difference between FromSqlRaw and FromSqlInterpolated. |
| 31 | [Working with JSON Columns](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch31-json-columns.html) | JSON_VALUE in SQL Server, jsonb in PostgreSQL. EF Core's ToJson() mapping, Dapper custom type handlers. |
| 32 | [SQL &harr; LINQ Cheat Sheet](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch32-cheat-sheet.html) | Quick reference: every SQL clause mapped to LINQ, EF, and Dapper. Type mappings, Fluent API reference, common patterns. |
| 33 | [Real-World E-Commerce Project](https://yousafzainasir9.github.io/SQL-To-CSharp-Book/ch33-real-world-project.html) | Complete walkthrough: Clean Architecture API with EF Core for writes, Dapper for reads. All patterns applied to one project. |

---

## How Every Chapter Works

Each chapter follows the same dual-thinking structure:

```
1. The SQL Way       →  Raw SQL showing the relational approach
2. LINQ Method       →  .Where().Select().OrderBy() chain syntax
3. LINQ Query        →  from x in db where x.Id > 5 select x
4. EF-Generated SQL  →  What the ORM actually sends to the database
```

This triple-comparison format ensures you understand the concept from every angle — not just how to write the code, but what's happening underneath.

---

## Who This Book Is For

**SQL developers moving to C#** — you already think in joins and subqueries. This book shows you the exact C# equivalent of what you already know.

**C# developers who struggle with databases** — you know LINQ but don't understand the SQL it generates. This book shows you what's happening on the other side.

**Full-stack developers** — you work with both sides daily. This book gives you the mental model to think fluently in either world.

---

## Tech Stack

The book covers C# with .NET 8, SQL Server as the primary database (with PostgreSQL notes where relevant), Entity Framework Core 8, and Dapper 2.x. All code examples compile and run against these versions.

---

## Running Locally

Clone the repository and open `index.html` in any browser — no build step required. The site is pure HTML/CSS with Google Fonts, designed to work as a static GitHub Pages site.

```bash
git clone https://github.com/yousafzainasir9/SQL-To-CSharp-Book.git
cd SQL-To-CSharp-Book
# Open index.html in your browser
```

---

## License

This project is open source. Feel free to use it for learning, share it with your team, or contribute improvements.

---

Built by [@yousafzainasir9](https://github.com/yousafzainasir9)
