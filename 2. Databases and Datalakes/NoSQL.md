Key Concepts
Modern applications generate:
•	massive data volumes, 
•	rapidly changing schemas, 
•	real-time interactions, 
•	high user concurrency, 
•	distributed workloads. 
Traditional relational databases can struggle with:
•	scalability, 
•	rigid schemas, 
•	join-heavy workloads, 
•	distributed architectures. 
NoSQL systems were designed to address these modern challenges.
________________________________________
Why NoSQL Emerged
NoSQL systems are typically:
•	non-relational, 
•	schema-flexible, 
•	cluster-friendly, 
•	horizontally scalable, 
•	optimised for modern web-scale workloads. 
Benefits include:
•	faster scaling, 
•	lower latency, 
•	improved flexibility, 
•	better handling of unstructured data. 
________________________________________
Real-World Performance Benefits
Industry examples included:
X (Twitter)
Reduced infrastructure costs significantly by moving from MySQL to Cassandra for tweets and timelines. 
LinkedIn
Reduced query latency from hours to seconds using a NoSQL key-value store. 
Airbnb
Reduced costs using MongoDB and DynamoDB for scalable storage. 
________________________________________
Scalability
NoSQL databases scale horizontally by:
•	distributing data across nodes, 
•	supporting clustered environments, 
•	reducing dependency on joins. 
This is particularly important for:
•	social media, 
•	IoT, 
•	recommendation systems, 
•	streaming applications. 
________________________________________
High-Quality Data Pipelines
Reliable pipelines should be:
•	resilient, 
•	idempotent, 
•	scalable, 
•	capable of frequent execution. 
Idempotency
Ensures rerunning a process does not create duplicate or inconsistent outputs.
Resiliency
Allows systems to recover from:
•	network failures, 
•	interrupted jobs, 
•	temporary outages. 
________________________________________
K3 — Data Normalisation Principles
KSB:
Data normalisation principles and the advantages they achieve in databases for data protection, redundancy, and inconsistent dependency.
Key Concepts
SQL databases rely heavily on:
•	normalisation, 
•	relationships, 
•	foreign keys, 
•	structured schemas. 
NoSQL databases intentionally move away from strict normalisation.
________________________________________
Denormalisation in NoSQL
NoSQL systems often store related data together within the same document.
Advantages:
•	fewer joins, 
•	faster reads, 
•	simplified retrieval, 
•	improved scalability. 
Trade-offs:
•	duplicated data, 
•	increased storage usage, 
•	harder consistency management. 
________________________________________
Flexible Schemas
Unlike SQL systems with predefined schemas, NoSQL databases may allow:
•	variable document structures, 
•	optional fields, 
•	evolving data models. 
This is useful when:
•	requirements change rapidly, 
•	data sources vary, 
•	structures evolve frequently. 
________________________________________
Relationship Management
NoSQL systems can still store relationships, but:
•	not typically through relational joins, 
•	often through embedded documents, 
•	or graph relationships. 
________________________________________
SQL vs NoSQL Structure
SQL
•	tables, 
•	rows, 
•	columns, 
•	foreign keys, 
•	relational integrity. 
MongoDB
•	collections, 
•	documents, 
•	fields, 
•	BSON objects. 
________________________________________
K5 — Risks, Ethics and Data Quality
KSB:
The inherent risks of data such as incomplete data, ethical data sources and how to ensure data quality.
Key Concepts
Flexible schemas improve agility but introduce risks including:
•	inconsistent structures, 
•	duplicated fields, 
•	unclear standards, 
•	reduced governance. 
________________________________________
Risks of Schema-Less Design
Potential problems include:
•	poor documentation, 
•	inconsistent field naming, 
•	missing validation, 
•	incompatible structures, 
•	difficult reporting. 
Without strong governance:
•	data quality deteriorates quickly. 
________________________________________
Data Integrity Trade-Offs
Some NoSQL systems prioritise:
•	speed, 
•	scalability, 
•	availability 
over:
•	strict transactional consistency. 
MongoDB examples included:
•	no joins, 
•	limited transaction handling, 
•	document size limits. 
This demonstrates the trade-offs engineers must understand.
________________________________________
Governance Challenges
Schema flexibility requires:
•	naming conventions, 
•	metadata standards, 
•	validation rules, 
•	monitoring processes. 
Otherwise organisations may struggle to:
•	interpret datasets, 
•	integrate systems, 
•	trust analytics outputs. 
________________________________________
Data Quality in Pipelines
High-quality pipelines improve:
•	consistency, 
•	reliability, 
•	operational confidence. 
________________________________________
K18 — Streaming, Batch and On-Demand Data Movement
KSB:
How to use streaming, batching and on-demand services to move data from one location to another.
Key Concepts
NoSQL technologies are heavily used in:
•	distributed pipelines, 
•	real-time ingestion, 
•	event-driven systems, 
•	scalable APIs, 
•	cloud-native applications. 
________________________________________
Data Pipelines
A data pipeline moves data through stages such as:
1.	Extract 
2.	Process/Transform 
3.	Analyse/Model 
4.	Present 
Pipelines support:
•	descriptive analytics, 
•	predictive analytics, 
•	exploratory analysis, 
•	operational systems. 
________________________________________
Pipeline Benefits
Benefits introduced included:
•	automation, 
•	efficiency, 
•	consistency, 
•	scalability, 
•	real-time insights. 
________________________________________
Real-Time Workloads
NoSQL systems are useful when applications require:
•	rapid reads/writes, 
•	high-frequency updates, 
•	low-latency APIs, 
•	streaming ingestion. 
________________________________________
Redis for Fast Access
Redis is an in-memory key-value database:
•	extremely fast, 
•	RAM-based, 
•	suitable for caching and sessions. 
Typical use cases:
•	dashboards, 
•	APIs, 
•	session stores, 
•	caching layers. 
________________________________________
Column-Based Databases
Column stores such as:
•	Cassandra, 
•	HBase 
are optimised for:
•	high-volume ingestion, 
•	analytics, 
•	distributed storage, 
•	sparse datasets. 
________________________________________
K27 — Descriptive, Predictive and Prescriptive Analytics
KSB:
The principles of descriptive, predictive and prescriptive analytics.
Key Concepts
NoSQL systems support modern analytics by handling:
•	large-scale datasets, 
•	semi-structured data, 
•	rapidly changing schemas, 
•	real-time data flows. 
________________________________________
Analytics-Oriented NoSQL Systems
Column-based databases are especially useful for:
•	data warehousing, 
•	analytics, 
•	reporting, 
•	web-scale processing. 
________________________________________
Graph Analytics
Graph databases specialise in:
•	relationship analysis, 
•	recommendation systems, 
•	social network modelling, 
•	fraud detection. 
Example
Finding:
•	“friends of friends” 
•	common interactions 
•	recommendation paths 
is much faster in graph databases than in highly normalised relational systems.
________________________________________
Recommendation Systems
Examples included:
•	Walmart product recommendations, 
•	Medium content personalisation, 
•	Cisco support analysis. 
These are examples of:
•	predictive analytics, 
•	recommendation engines, 
•	behavioural analysis. 
________________________________________
NLP Pipelines
An NLP (Natural Language Processing) pipeline example demonstrated how unstructured text data can be:
•	extracted, 
•	transformed, 
•	analysed, 
•	modelled. 
________________________________________
S7 — Working with SQL, NoSQL and Distributed Data Stores
KSB:
Work with different types of data stores, such as SQL, NoSQL, and distributed file system.
Key Concepts
Four major NoSQL database categories were introduced:
Type	Example	Best Use
Key-value	Redis	Fast caching/session storage
Document	MongoDB	Flexible semi-structured data
Column-based	Cassandra/HBase	Large-scale analytics
Graph	Neo4j	Relationship-heavy systems
________________________________________
Key-Value Databases
Store:
•	simple key-value pairs, 
•	dictionary-like structures. 
Advantages:
•	extremely fast, 
•	simple retrieval, 
•	low latency. 
________________________________________
Document Databases
MongoDB stores:
•	JSON/BSON documents, 
•	nested structures, 
•	flexible schemas. 
Useful when:
•	structures change often, 
•	rapid ingestion is needed, 
•	joins are unnecessary. 
________________________________________
Column-Based Databases
Optimised for:
•	analytical workloads, 
•	warehousing, 
•	sparse datasets, 
•	cloud scalability. 
________________________________________
Graph Databases
Store:
•	nodes, 
•	edges, 
•	relationships. 
Optimised for:
•	graph traversal, 
•	connected data, 
•	recommendation systems. 
________________________________________
MongoDB Terminology
SQL	MongoDB
Table	Collection
Row	Document
Column	Field
________________________________________
S15 — Optimising Data Ingestion
KSB:
Optimise data ingestion processes using batch, streaming and on-demand frameworks.
Key Concepts
NoSQL systems are commonly used in ingestion pipelines because they support:
•	rapid writes, 
•	distributed scaling, 
•	flexible schemas, 
•	semi-structured data ingestion. 
________________________________________
MongoDB Querying
Examples included:
db.collection.find()
Filtering:
db.collection.find({Artist:"Nirvana"})
Sorting:
db.collection.find().sort({Title:1})
________________________________________
MongoDB with Python
MongoDB can be accessed using:
•	PyMongo, 
•	cursors, 
•	iterative query processing. 
________________________________________
Cursor-Based Retrieval
Find operations return cursors:
•	allowing scalable iteration through result sets, 
•	supporting efficient retrieval of large datasets. 
________________________________________
Writing Data Efficiently
MongoDB simplifies insertion by storing nested data in a single document.
Compared to SQL:
•	fewer inserts, 
•	fewer joins, 
•	simpler write operations. 
________________________________________
Flexible Ingestion Design
Document databases are useful when:
•	schemas evolve rapidly, 
•	ingestion speed matters, 
•	data formats vary frequently. 
________________________________________
Overall Understanding
NoSQL databases were created to solve modern data engineering challenges involving:
•	scalability, 
•	flexibility, 
•	distributed systems, 
•	high-volume ingestion, 
•	and unstructured data. 
Different NoSQL technologies serve different purposes:
•	Redis for speed, 
•	MongoDB for flexible documents, 
•	Cassandra for analytics scale, 
•	Neo4j for relationships. 
Modern data engineers must understand:
•	trade-offs between SQL and NoSQL, 
•	schema flexibility, 
•	denormalisation, 
•	distributed architectures, 
•	scalable pipelines, 
•	and real-time data systems. 
Choosing the correct database technology depends on:
•	workload patterns, 
•	query requirements, 
•	scalability needs, 
•	consistency requirements, 
•	and business objectives.

