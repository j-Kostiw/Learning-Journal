Key Concepts

Modern organisations rely on data products that must be:

available,
reliable,
scalable,
performant,
and trustworthy.

Data engineers are responsible for building systems that:

move data efficiently,
maintain uptime,
support analytics,
and ensure business users can access accurate information when needed.

Examples discussed included:

Netflix recommendation systems,
HR analytics dashboards,
cloud-based data platforms.
Data Engineering Responsibilities

Data engineers support performance by:

designing efficient ETL/ELT pipelines,
monitoring pipeline failures,
validating incoming data,
reducing bottlenecks,
scaling infrastructure for growing datasets.
Important Supporting Concepts
Big Data Challenges

As data grows:

systems slow down,
storage becomes difficult,
queries become expensive,
poor architecture causes missed business opportunities.

This explains why monitoring and optimisation are essential.

AWS Well-Architected Framework

Cloud engineering standards help ensure:

reliability,
operational excellence,
security,
performance efficiency,
cost optimisation.

These principles underpin enterprise-grade data products.

Practical Understanding

Examples of optimisation:

partitioning large datasets,
indexing databases,
caching frequent queries,
using distributed storage,
scaling compute resources automatically.
K3 — Data Normalisation Principles

KSB:
Data normalisation principles and the advantages they achieve in databases for data protection, redundancy, and inconsistent dependency.

Key Concepts

Structured data systems often rely on relational databases where data is organised into tables.

Normalisation helps:

reduce duplication,
improve consistency,
avoid update anomalies,
improve maintainability.
Why Normalisation Matters

Without normalisation:

the same data may exist in multiple places,
updates become inconsistent,
storage is wasted,
relationships become unreliable.
Example

If employee department names are stored repeatedly in every record:

spelling inconsistencies occur,
updates become difficult,
duplicate data increases.

A normalised design separates:

employee data,
department data,
salary data,
into linked tables.
Connection to Data Quality

Normalisation supports:

cleaner datasets,
more reliable analytics,
improved governance,
easier validation.
Engineering Context

Data engineers regularly:

design schemas,
transform raw data into structured formats,
integrate datasets from multiple systems,
optimise databases for analytics workloads.
Data Formats

Different formats were referenced:

CSV,
JSON,
XML.

These formats often require transformation and modelling before being loaded into structured systems.

K5 — Risks, Ethics and Data Quality

KSB:
The inherent risks of data such as incomplete data, ethical data sources and how to ensure data quality.

Key Concepts

Data is only valuable when it is:

accurate,
complete,
trustworthy,
ethical,
and properly governed.
The 5 Vs of Big Data

Important characteristics include:

Volume,
Variety,
Velocity,
Veracity,
Value.
Veracity

Veracity refers to:

accuracy,
reliability,
trustworthiness of data.

Poor veracity leads to:

incorrect analytics,
misleading dashboards,
bad business decisions.
Data Quality Risks

Common risks include:

incomplete records,
duplicate data,
inconsistent formatting,
missing values,
outdated information,
biased datasets.
Example

An HR analytics system with inaccurate employee records may:

incorrectly predict resignations,
misclassify performance,
create unfair outcomes.
Data Stewardship Principles

Three important principles:

Data Quality
Data Governance
Data Ethics
Governance

Governance ensures:

ownership,
accountability,
compliance,
auditability.
Ethics

Ethical data practice includes:

using lawful data sources,
avoiding algorithmic bias,
protecting user privacy,
ensuring transparency.
Regulatory Standards
GDPR

The General Data Protection Regulation requires:

lawful processing,
consent,
data minimisation,
secure handling of personal information.
ISO 27001

Provides frameworks for:

information security,
risk management,
access control,
secure operational processes.
Practical Data Quality Methods

Data engineers improve quality through:

validation checks,
schema enforcement,
deduplication,
anomaly detection,
logging and monitoring,
automated testing.
K18 — Streaming, Batch and On-Demand Data Movement

KSB:
How to use streaming, batching and on-demand services to move data from one location to another.

Key Concepts

Data pipelines move information between:

applications,
databases,
APIs,
cloud platforms,
analytics systems.

Three major approaches were introduced.

1. Batch Processing

Batching processes data:

at scheduled intervals,
in groups,
often overnight or hourly.
Example

Daily payroll processing.

Advantages
efficient for large volumes,
cheaper to run,
easier to manage.
Limitations
not real-time,
delayed insight delivery.
2. Streaming

Streaming processes data continuously in near real time.

Example
social media feeds,
banking transactions,
sensor monitoring,
Netflix recommendations.
Advantages
immediate insight,
rapid alerts,
real-time analytics.
Challenges
infrastructure complexity,
scaling requirements,
fault tolerance needs.
3. On-Demand Processing

Triggered when required by users or systems.

Example

A dashboard refreshing when opened.

Advantages
flexible,
efficient for unpredictable workloads.
Data Engineering Activities

Typical activities include:

collecting data from multiple sources,
transforming formats,
validating quality,
integrating into unified datasets.

Example integration sources included:

CSV employee reviews,
SQL databases,
JSON survey responses.
K27 — Descriptive, Predictive and Prescriptive Analytics

KSB:
The principles of descriptive, predictive and prescriptive analytics.

1. Descriptive Analytics

Answers:

“What happened?”

Uses:

dashboards,
reports,
KPIs,
summaries.
Example

Monthly employee turnover reports.

2. Predictive Analytics

Answers:

“What is likely to happen?”

Uses:

machine learning,
forecasting,
probability modelling.
Example

Predicting whether employees may resign.

Decision trees were introduced as a predictive model:

interpretable,
rule-based,
easy to visualise.

Decision factors included:

salary,
satisfaction,
promotion history,
workload.
3. Prescriptive Analytics

Answers:

“What should we do?”

Uses predictions to recommend actions.

Example

If an employee is likely to leave:

offer promotion,
reduce workload,
improve engagement.
Analytics Lifecycle

Three stages of adding value with data:

1. Data Wrangling
sourcing,
cleaning,
preparation.
2. Data Exploration
experimentation,
analytics,
model building.
3. Data Operationalisation
deployment,
dashboards,
automation,
business strategy.

Data engineers contribute heavily to:

wrangling,
infrastructure,
operationalisation.
S7 — Working with SQL, NoSQL and Distributed Data Stores

KSB:
Work with different types of data stores, such as SQL, NoSQL, and distributed file system.

SQL Databases

Relational systems using:

tables,
schemas,
structured queries.

Best for:

transactional systems,
structured data,
strong consistency.
Example

Employee records database.

NoSQL Databases

Designed for:

flexible schemas,
semi-structured data,
high scalability.

Best for:

large-scale web systems,
streaming platforms,
rapidly changing data.
Common Types
document stores,
key-value stores,
graph databases,
column-family databases.

JSON data commonly appears in NoSQL systems.

Distributed File Systems

Used for massive-scale storage across multiple machines.

Designed for:

fault tolerance,
scalability,
parallel processing.
Example Technologies
Hadoop HDFS,
cloud object storage,
distributed data lakes.
Why Multiple Data Stores Matter

Modern systems rarely use one storage type.

A single organisation may combine:

SQL databases for finance,
NoSQL for web applications,
distributed storage for analytics.

Data engineers must understand:

interoperability,
transformation,
integration patterns.
S15 — Optimising Data Ingestion

KSB:
Optimise data ingestion processes using batch, streaming and on-demand frameworks.

Key Concepts

Data ingestion is the process of:

collecting,
importing,
transferring,
and loading data into systems.

Efficient ingestion is critical because poor ingestion causes:

delays,
bottlenecks,
inaccurate reporting,
failed analytics.
Batch Ingestion

Best for:

scheduled workloads,
historical datasets,
large-volume processing.

Optimisation techniques:

parallel processing,
compression,
partitioning,
incremental loads.
Streaming Ingestion

Best for:

real-time analytics,
fraud detection,
monitoring systems.

Optimisation techniques:

event buffering,
distributed consumers,
checkpointing,
autoscaling.
On-Demand Ingestion

Used when:

users request data dynamically,
APIs are queried interactively.

Optimisation techniques:

caching,
asynchronous processing,
query optimisation.
Data Pipeline Optimisation

Important engineering considerations:

throughput,
latency,
reliability,
scalability,
fault tolerance.
Data Quality During Ingestion

Ingestion pipelines should include:

validation rules,
schema checks,
duplicate detection,
logging,
monitoring alerts.
Overall Understanding

The session establishes that data engineering is not only about moving data. It involves:

building scalable systems,
ensuring quality and ethics,
enabling analytics,
supporting business strategy,
and delivering reliable data products.

A successful data engineer combines:

technical capability,
governance awareness,
optimisation skills,
and business understanding.
