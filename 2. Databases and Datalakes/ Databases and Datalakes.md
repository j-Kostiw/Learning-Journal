Database administration is essential for:
•	maintaining performance, 
•	ensuring availability, 
•	protecting data integrity, 
•	reducing outages, 
•	supporting scalability, 
•	and enabling efficient analytics. 
The session focused on:
•	profiling, 
•	optimisation, 
•	indexing, 
•	recovery, 
•	monitoring, 
•	and operational resilience. 
________________________________________
Data Profiling
Data profiling analyses existing datasets to determine:
•	structure, 
•	content, 
•	quality, 
•	consistency, 
•	metadata accuracy. 
It helps organisations identify:
•	inaccurate values, 
•	missing data, 
•	schema inconsistencies, 
•	rule violations, 
•	duplicate records. 
________________________________________
Data Quality Monitoring
Data quality monitoring forms part of a wider quality improvement programme involving:
•	data discovery, 
•	correction, 
•	prevention, 
•	monitoring, 
•	incident investigation. 
This supports reliable enterprise reporting and analytics.
________________________________________
Query Profiling
Query profiling gathers detailed execution information to identify:
•	slow-running queries, 
•	bottlenecks, 
•	inefficient logic, 
•	excessive resource usage. 
Common profiling tools:
•	MySQL: EXPLAIN, SHOW PROFILE 
•	PostgreSQL: EXPLAIN ANALYZE 
•	SQL Server execution plans. 
________________________________________
Query Execution Analysis
Profiling includes:
1.	Collecting execution data 
2.	Analysing execution plans 
3.	Monitoring CPU, memory and I/O 
4.	Identifying bottlenecks. 
Common Performance Problems
•	full table scans, 
•	missing indexes, 
•	expensive joins, 
•	inefficient subqueries. 
________________________________________
Query Optimisation
Optimisation improves:
•	retrieval speed, 
•	throughput, 
•	scalability, 
•	resource efficiency. 
Techniques include:
•	indexing, 
•	rewriting queries, 
•	partitioning, 
•	caching, 
•	denormalisation, 
•	configuration tuning. 
________________________________________
Indexing
Indexes are critical for performance.
Important principle:
“If you’re not indexing, you’re not close to full performance.” 
Indexes help:
•	WHERE filtering, 
•	joins, 
•	sorting, 
•	range queries. 
Example:
CREATE INDEX idx_department_id
ON employees(department_id);
________________________________________
Partitioning
Partitioning divides large tables into smaller logical sections.
Benefits:
•	reduced scanning, 
•	faster queries, 
•	improved maintenance, 
•	better scalability. 
________________________________________
Caching
Caching stores frequently accessed data in memory.
Benefits:
•	reduced database load, 
•	lower latency, 
•	improved responsiveness. 
________________________________________
Configuration Tuning
Database configuration settings can be adjusted for:
•	memory allocation, 
•	buffer sizes, 
•	workload optimisation. 
________________________________________
K3 — Data Normalisation Principles
KSB:
Data normalisation principles and the advantages they achieve in databases for data protection, redundancy, and inconsistent dependency.
Key Concepts
Data profiling helps identify:
•	denormalisation, 
•	inconsistent relationships, 
•	dependency problems, 
•	invalid data structures. 
________________________________________
Row and Multi-Table Examination
Profiling examines:
•	primary key candidates, 
•	foreign key relationships, 
•	multi-column dependencies, 
•	NULL dependencies, 
•	relationship cardinality. 
This helps maintain:
•	referential integrity, 
•	relational consistency, 
•	structured schemas. 
________________________________________
Third Normal Form Discovery
Vendor profiling tools may support:
•	third normal form discovery, 
•	foreign key discovery, 
•	pattern recognition. 
This improves:
•	schema quality, 
•	maintainability, 
•	integration reliability. 
________________________________________
Denormalisation Trade-Offs
Denormalisation may sometimes improve performance by reducing joins. 
However, trade-offs include:
•	duplicated data, 
•	storage growth, 
•	increased update complexity, 
•	potential inconsistency. 
Data engineers must balance:
•	query speed, 
•	integrity, 
•	scalability. 
________________________________________
K5 — Risks, Ethics and Data Quality
KSB:
The inherent risks of data such as incomplete data, ethical data sources and how to ensure data quality.
Key Concepts
Data quality problems create risks including:
•	incorrect analytics, 
•	operational failures, 
•	compliance breaches, 
•	customer dissatisfaction, 
•	legal exposure. 
The session highlighted that:
Data quality problems can cost companies 15–25% of bottom-line profit. 
________________________________________
Invalid Data Detection
Profiling identifies:
•	missing values, 
•	out-of-range values, 
•	invalid combinations, 
•	inconsistent formats, 
•	suspicious records. 
Examples included:
•	fake names, 
•	invalid addresses, 
•	inconsistent date formats. 
________________________________________
Metadata and Data Rules
Good metadata defines:
•	valid values, 
•	formats, 
•	relationships, 
•	business rules. 
Profiling validates:
•	metadata accuracy, 
•	adherence to rules, 
•	hidden dependencies. 
________________________________________
Data Governance
Data rules exist:
•	whether documented or not, 
•	whether enforced or not. 
This highlights the importance of:
•	governance, 
•	stewardship, 
•	standards enforcement, 
•	monitoring. 
________________________________________
Security Best Practices
Security guidance included:
•	avoid shared logins, 
•	protect user IDs, 
•	separate DBA and developer access, 
•	avoid embedding privileged credentials in applications. 
These practices reduce:
•	insider threats, 
•	accidental misuse, 
•	unauthorised access. 
________________________________________
Human Error and Outages
Human error was identified as the leading cause of datacentre outages (~70%). 
Examples included:
•	deleting production databases, 
•	incorrect hardware removal, 
•	unauthorised repairs. 
________________________________________
Operational Transparency
Major companies maintain trust during outages by:
•	publishing updates, 
•	providing dashboards, 
•	issuing post-mortems, 
•	communicating clearly. 
This reflects good operational governance.
________________________________________
K18 — Streaming, Batch and On-Demand Data Movement
KSB:
How to use streaming, batching and on-demand services to move data from one location to another.
Key Concepts
Operational databases continuously move data between:
•	transactional systems, 
•	warehouses, 
•	analytics platforms, 
•	archive environments, 
•	backup systems. 
________________________________________
Database Archiving
Database archiving removes inactive data from operational systems and stores it separately for long-term retention. 
Benefits:
•	reduced operational load, 
•	lower storage cost, 
•	improved query performance, 
•	simplified recovery. 
________________________________________
Archive Architecture
The archive architecture included:
•	operational systems, 
•	archive servers, 
•	extractors, 
•	archive storage, 
•	archive catalogues. 
Processes include:
•	extraction, 
•	storage, 
•	validation, 
•	retention management, 
•	audit tracking. 
________________________________________
Data Retention
Retention requirements are driven by:
•	business rules, 
•	legal regulations, 
•	compliance obligations. 
Retention periods may exceed:
•	10, 
•	25, 
•	50, 
•	or even 70 years. 
________________________________________
Archive Extraction
Archive extractors should:
•	avoid operational disruption, 
•	support recovery, 
•	maintain audit logs, 
•	ensure transactional consistency. 
________________________________________
K27 — Descriptive, Predictive and Prescriptive Analytics
KSB:
The principles of descriptive, predictive and prescriptive analytics.
Key Concepts
Analytics reliability depends on:
•	clean data, 
•	efficient databases, 
•	accurate metadata, 
•	performant queries. 
________________________________________
Improved Analytic Results
High-quality data improves:
•	decision-making, 
•	forecasting, 
•	reporting, 
•	operational insights. 
________________________________________
Profiling for Analytics
Profiling functions support analytics by:
•	detecting outliers, 
•	measuring distributions, 
•	calculating aggregates, 
•	identifying relationships. 
Examples:
•	AVG, 
•	SUM, 
•	MEDIAN, 
•	standard deviation. 
________________________________________
Query Optimisation for Reporting
Optimised queries improve:
•	dashboard speed, 
•	warehouse reporting, 
•	BI responsiveness, 
•	analytics scalability. 
________________________________________
Data Warehousing Support
Profiling supports warehouses by:
•	cleansing data in transit, 
•	improving integration quality, 
•	validating transformations. 
________________________________________
S7 — Working with SQL, NoSQL and Distributed Data Stores
KSB:
Work with different types of data stores, such as SQL, NoSQL, and distributed file system.
Key Concepts
The topic focused primarily on relational database administration but also covered enterprise-scale storage environments.
________________________________________
Archive Storage Environments
Examples included:
•	DB2, 
•	IMS, 
•	Oracle, 
•	SAP, 
•	PeopleSoft. 
These represent enterprise operational systems used in:
•	finance, 
•	ERP, 
•	government, 
•	healthcare, 
•	enterprise analytics. 
________________________________________
Metadata Management
Archive designers must define:
•	metadata, 
•	business records, 
•	storage formats, 
•	retention policies, 
•	reference data. 
________________________________________
Multi-Table Profiling
Profiling across tables helps engineers:
•	identify foreign keys, 
•	validate schemas, 
•	map relationships, 
•	discover dependencies. 
________________________________________
S15 — Optimising Data Ingestion
KSB:
Optimise data ingestion processes using batch, streaming and on-demand frameworks.
Key Concepts
Database optimisation directly affects ingestion efficiency.
Poorly optimised systems create:
•	slow ETL jobs, 
•	pipeline bottlenecks, 
•	excessive resource usage, 
•	failed analytics workloads. 
________________________________________
Efficient Query Design
Important optimisation rule:
NEVER use SELECT * unnecessarily. 
Selecting only required columns:
•	reduces I/O, 
•	improves network performance, 
•	lowers memory usage. 
________________________________________
Query Rewriting
Queries should be simplified where possible:
•	optimise joins, 
•	reduce nested subqueries, 
•	minimise scans. 
________________________________________
Recovery and Availability
Recovery models determine:
•	backup behaviour, 
•	restore options, 
•	recovery granularity. 
Simple Recovery
•	restore latest backup only. 
Full Recovery
•	restore to earlier points before failure. 
________________________________________
Point-in-Time Recovery (PITR)
PITR combines:
•	snapshots, 
•	transaction logging, 
•	automation. 
Benefits:
•	precise recovery, 
•	improved availability, 
•	disaster resilience. 
________________________________________
Amazon RDS Snapshots
Snapshot types:
•	automated snapshots, 
•	manual snapshots. 
Used for:
•	backups, 
•	disaster recovery, 
•	rollback, 
•	migration. 
________________________________________
Overall Understanding
Database administration is a core responsibility in enterprise data engineering.
Data engineers must understand:
•	data profiling, 
•	query optimisation, 
•	indexing, 
•	archiving, 
•	recovery, 
•	retention, 
•	security, 
•	operational resilience, 
•	and outage management. 
Reliable databases require continuous:
•	monitoring, 
•	tuning, 
•	profiling, 
•	governance, 
•	and optimisation. 
The ultimate goal is to ensure:
•	high availability, 
•	scalable performance, 
•	trustworthy analytics, 
•	secure data handling, 
•	and resilient enterprise operations. 
