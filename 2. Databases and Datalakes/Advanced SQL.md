[L5DE M2T3 v1.pdf](https://github.com/user-attachments/files/19410527/L5DE.M2T3.v1.pdf)
Key Concepts

Advanced SQL techniques are essential for:

database optimisation,
efficient querying,
scalable reporting,
high-performance analytics,
and reliable enterprise systems.

The session introduced:

query optimisation,
indexes,
aggregation,
views,
and efficient data retrieval strategies.
Database Performance Optimisation

Large datasets create performance challenges because:

sequential scans become slow,
joins increase complexity,
aggregations consume resources,
poorly indexed systems scale badly.

Data engineers optimise systems by:

indexing,
reducing unnecessary scans,
structuring efficient joins,
using materialised views,
minimising redundant processing.
Indexes

Indexes improve query speed by reducing the amount of data scanned.

Example:

CREATE INDEX nameIndex ON Person(name)

Indexes are particularly useful for:

search operations,
filtering,
joins,
range queries.
B+ Tree Indexing

B+ Trees were introduced as a common indexing structure.

Benefits:

fast lookup performance,
efficient sorting,
improved range query execution,
reduced disk access.

Example range query:

SELECT *
FROM Person
WHERE age > 25 AND age < 28

Composite Indexes

Indexes can span multiple columns:

CREATE INDEX doubleindex ON Person(age, city)

Useful when queries filter on:

multiple attributes together.

Example:

WHERE age = 55 AND city = "Southampton"
Materialised Views

Materialised views improve runtime performance because:

results are precomputed,
expensive queries are cached,
reporting becomes faster.

Trade-off:

data may become stale if not refreshed.
K3 — Data Normalisation Principles

KSB:
Data normalisation principles and the advantages they achieve in databases for data protection, redundancy, and inconsistent dependency.

Key Concepts

Advanced SQL depends heavily on:

structured schemas,
relationships between tables,
referential integrity,
and well-designed relational databases.
Relational Database Structure

Examples used tables such as:

Person,
Product,
Purchase,
Employee,
Author,
Wrote.

These demonstrate relational modelling where:

entities are separated logically,
relationships are maintained using keys,
redundancy is reduced.
JOIN Operations

JOINs connect related tables using shared attributes.

This is fundamental to normalised database design.

INNER JOIN

Returns only matching records:

SELECT *
FROM table_A
INNER JOIN table_B
ON table_A.A = table_B.A;

Useful for:

combining related datasets,
enforcing relational consistency.
LEFT and RIGHT JOIN

LEFT JOIN:

keeps all records from the left table,
fills unmatched records with NULL values.

RIGHT JOIN:

keeps all records from the right table.

These joins help identify:

missing relationships,
incomplete datasets,
orphaned records.
CROSS JOIN

Produces a Cartesian product:

every row from one table paired with every row from another.

Can create very large result sets.

Useful cautiously in:

combinational analysis,
testing,
matrix generation.
UNION

Combines results from multiple SELECT statements.

Rules:

same number of columns,
compatible data types,
same column order.

Useful for:

merging datasets,
consolidating sources,
federated reporting.
K5 — Risks, Ethics and Data Quality

KSB:
The inherent risks of data such as incomplete data, ethical data sources and how to ensure data quality.

Key Concepts

SQL querying introduces risks if:

joins are incorrect,
NULL values are mishandled,
aggregations are misunderstood,
views expose sensitive data,
schemas change unexpectedly.
NULL Handling

Outer joins often generate NULL values where no relationship exists.

Example:

unmatched employee records,
missing product mappings,
incomplete transactions.

Data engineers must:

validate outputs,
handle NULL safely,
avoid misleading analytics.
Data Integrity

Relational joins depend on:

accurate keys,
valid relationships,
consistent identifiers.

Poor schema quality can lead to:

duplicate results,
incorrect aggregations,
data inconsistency.
Views and Access Control

Views support security and governance by limiting visible data.

Example:

CREATE VIEW Developers AS
SELECT name, project
FROM Employee
WHERE department = "Development"

This allows:

restricted access,
role-based visibility,
safer data sharing.
Risks with Updating Views

Some views cannot safely support updates because:

data originates from multiple tables,
aggregations exist,
DISTINCT is used,
GROUP BY is applied.

These are called:

non-updatable views.
Schema Evolution Risks

DDL operations such as:

ALTER TABLE
DROP age;

can impact:

applications,
reports,
integrations,
stored procedures.

Schema changes must therefore be managed carefully.

K18 — Streaming, Batch and On-Demand Data Movement

KSB:
How to use streaming, batching and on-demand services to move data from one location to another.

Key Concepts

SQL operations are foundational for:

ETL pipelines,
batch processing,
data warehouse loading,
transformation workflows.
Aggregation in Batch Analytics

Aggregation operations support large-scale reporting.

Examples:

SUM
COUNT
AVG
MIN
MAX

Used for:

KPIs,
dashboards,
operational reporting,
warehouse summaries.
GROUP BY Processing

GROUP BY enables aggregation across categories.

Example:

SELECT product,
SUM(price * quantity) AS TotalSales
FROM Purchase
GROUP BY product;

Useful for:

sales reporting,
customer segmentation,
operational analytics.
HAVING Clause

HAVING filters groups after aggregation.

Example:

HAVING SUM(quantity) > 100

Difference:

WHERE filters rows before grouping,
HAVING filters aggregated groups afterward.
Query Execution Order

The session explained SQL execution stages:

FROM
WHERE
GROUP BY
HAVING
SELECT

Understanding execution order helps engineers:

optimise queries,
troubleshoot logic,
reduce computational overhead.
K27 — Descriptive, Predictive and Prescriptive Analytics

KSB:
The principles of descriptive, predictive and prescriptive analytics.

Key Concepts

Advanced SQL powers descriptive analytics through:

aggregation,
summarisation,
grouping,
filtering,
reporting.
Descriptive Analytics

Examples:

total sales by product,
customer counts,
purchase trends,
category reporting.

SQL aggregations help answer:

“What happened?”

Aggregation Functions
SUM

Calculates totals.

COUNT

Counts rows or values.

AVG

Calculates averages.

MIN/MAX

Find smallest or largest values.

These functions are heavily used in:

BI dashboards,
operational reporting,
warehouse analytics.
DISTINCT Aggregation

Example:

COUNT(DISTINCT category)

Useful for:

unique customer counts,
category analysis,
deduplication.
Nested Queries vs GROUP BY

The session compared:

nested subqueries,
grouped aggregation.
Expert SQL Style

Using GROUP BY is often:

cleaner,
faster,
more scalable.

Example:

GROUP BY Author.name
HAVING COUNT(Wrote.url) > 10

S7 — Working with SQL, NoSQL and Distributed Data Stores

KSB:
Work with different types of data stores, such as SQL, NoSQL, and distributed file system.

Key Concepts

This topic focused heavily on relational SQL systems and structured storage models.

Data Definition Language (DDL)

DDL manages database structure.

Examples include:

CREATE TABLE,
ALTER TABLE,
DROP TABLE,
CREATE INDEX.
SQL Data Types

Examples included:

VARCHAR,
CHAR,
INT,
REAL,
DATE,
DATETIME.

Choosing appropriate types improves:

storage efficiency,
validation,
performance,
interoperability.
Schema Design

Example schema:

CREATE TABLE Person(
 name VARCHAR(30),
 social-security-number INT,
 age SHORTINT,
 city VARCHAR(30)
);

This reinforces:

structured modelling,
domain consistency,
relational design principles.
Domains

Reusable domains improve standardisation.

Example:

CREATE DOMAIN address AS VARCHAR(55)

Benefits:

consistent validation,
reusable schema logic,
improved maintainability.
Views as Virtual Tables

Views create reusable logical datasets.

Benefits:

abstraction,
security,
simplified querying,
reusable business logic.
S15 — Optimising Data Ingestion

KSB:
Optimise data ingestion processes using batch, streaming and on-demand frameworks.

Key Concepts

Efficient SQL processing supports ingestion pipelines by:

reducing transformation overhead,
optimising joins,
improving aggregation performance,
structuring scalable warehouse queries.
Efficient Query Design

Efficient SQL avoids:

unnecessary nested queries,
redundant scans,
Cartesian products,
excessive joins.
GROUP BY Optimisation

GROUP BY operations are computationally expensive on large datasets.

Optimisation strategies:

indexing grouped columns,
partitioning datasets,
pre-aggregation,
materialised views.
Nested Queries vs Aggregation

The session demonstrated that:

GROUP BY solutions are often more efficient than repeated subqueries.

This matters because:

nested queries may repeatedly scan large tables,
grouped queries process datasets more efficiently.
Data Warehouse Optimisation

Materialised views are commonly used in warehouses because they:

precompute heavy calculations,
speed up dashboards,
reduce query latency.
Maintaining Query Performance

Performance monitoring considerations include:

index usage,
execution plans,
query cost,
storage design,
schema evolution.
Overall Understanding

Advanced SQL is fundamental to enterprise data engineering because it enables:

scalable querying,
efficient aggregation,
relational modelling,
performance optimisation,
secure data access,
and reliable analytics.

Modern data engineers must understand:

joins,
grouping,
indexing,
schema design,
views,
query optimisation,
and aggregation strategies

to build performant, scalable, maintainable data systems.
