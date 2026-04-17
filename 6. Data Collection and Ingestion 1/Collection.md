How data is sourced, collected, cleaned, and ingested into systems for use

Everything downstream (analytics, ML, dashboards) depends on this being done correctly.

2. Key Concepts from Slides
Data Collection vs Data Ingestion

From recap discussion (page 7) :

Clear distinction (EPA critical):
Data Collection
→ Gathering data from sources
(APIs, databases, sensors, files)
Data Ingestion
→ Moving data into a system for storage/processing
(pipelines, ETL, streaming)
EPA Tip

A strong answer always separates:

“Where data comes from” vs “How it enters the system”

ETL as Best Practice

From knowledge check (page 4) :

Correct approach:

Use ETL (Extract, Transform, Load) before loading into a warehouse

Why this matters:
Ensures data quality
Standardises formats
Removes errors early
Weak approaches (avoid):
Load everything raw without checks
Clean data later (costly and inefficient)
KSB Mapping
K4 / K5 – Data processing concepts
S2 / S3 – Data pipeline design
Automation in Data Pipelines

From objectives (page 5) :

Why automation matters:
Reduces human error
Improves scalability
Enables real-time processing
Example:
Scheduled ingestion jobs
Streaming pipelines
KSB Mapping
S5 – Building pipelines
B2 – Efficiency mindset
Data Cleaning (Critical Skill)

From summary (page 19) :

Common techniques:
Remove duplicates
Handle missing values
Standardise formats
EPA Insight:

Bad data = bad decisions

KSB Mapping
K4 – Data quality
S2 – Data preparation
Pre-processing for Machine Learning

From summary (page 19) :

Key steps:
Normalisation
Encoding categorical variables
Feature scaling
Why it matters:
Improves model performance
Ensures consistency
3. Practical Data Engineering Design
Step 1 – Stakeholder Requirements

From page 13 :

What you must do:
Engage stakeholders
Define business objectives
Example:
Marketing → customer behaviour
Operations → inventory data
EPA Tip:

Always link:

Data → Business need

Step 2 – Data Assessment (The 4 Vs)

From page 13 :

Volume – how much data
Variety – types of data
Velocity – speed of data
Veracity – quality
Insight:

These determine:

Storage choice
Processing method
Step 3 – System Selection

From page 13 :

When to use each:
SQL databases
→ Structured data, transactions
NoSQL
→ Flexible, unstructured data
Data Lakes
→ Raw, large-scale data
Data Warehouses
→ Analytics and reporting
Clusters
→ Distributed processing
EPA Tip:

Always justify your choice

Step 4 – Data Acquisition Strategy

From page 14 :

Sources:
APIs
Web scraping
IoT devices
Third-party datasets
Include:
Data quality checks
Initial transformations
Step 5 – Data Management & Governance

From page 14 :

Key areas:
Access control
Compliance
Backup & recovery
Lifecycle management
KSB Mapping
K8 / K10 – Governance & security
B1 – Responsibility
Step 6 – Monitoring & Evaluation

From page 14 :

You must:
Monitor data quality
Track system performance
Adjust pipelines
4. Data Architecture (VERY IMPORTANT)
Common Folder Structure

From page 15 :

Typical pipeline flow:
Landing Area
Raw data
No processing
Staging Area
Initial cleaning
Ingestion Layer
Transformation + structuring
Archive
Long-term storage
EPA Insight:

This shows data lifecycle understanding

5. Case Study – E-commerce System Design

From pages 16–17 :

Business Objective
Improve customer experience
Optimise inventory
Data Design (Strong Example)
Data Types:
Customer → structured + unstructured
Inventory → structured
System Choices:
NoSQL → customer data
SQL → inventory
Data warehouse → analytics
Data Ingestion:
APIs, forms, POS systems
Data Management:
Governance policies
Real-time updates
Implementation:
MongoDB + PostgreSQL + Redshift
Monitoring:
Dashboards for KPIs
Why This is a Strong Answer

It shows:

Business alignment
Correct tech choices
Full pipeline thinking
KSB Mapping
S5 / S6 – System design
K7 – Architecture
6. Python & Practical Skills

From page 9 :

Key pandas skills:
.melt() → reshape data
.rename() → clean columns
.apply() → transformations
.to_numeric() → fix data types
Lambda Functions (Page 10)
Definition:

Small, anonymous functions for quick transformations

Example:

lambda y: y*y*y
When to use:
Simple transformations
Inline operations
7. Data Sources

From page 12 :

Examples:
Kaggle
Google Dataset Search
EPA Tip:

Mention real sources to strengthen answers

8. Data Licensing & Compliance

From page 18 :

Key responsibilities:
Understand usage rights
Track data usage
Ensure compliance
Train teams
Why it matters:
Legal risk
Ethical responsibility
KSB Mapping
K10 – Governance
B1 – Ethical practice
9. What Examiners Are Looking For
1. End-to-End Thinking

Not just:

“Load data”

But:

“Collect → clean → transform → store → monitor”

2. Justification

Always explain:

Why a tool is used
Why a method is chosen
3. Business Alignment

Every technical decision should answer:

“What problem does this solve?”

4. Data Quality Awareness

Show:

Cleaning
Validation
Monitoring
10. Final Takeaways

From summary (page 19) :

Automation improves efficiency
Data cleaning is essential
Pre-processing supports ML
Practical skills (Python, pandas) are critical
11. EPA Revision Checklist

You should be able to:

Explain data collection vs ingestion
Describe ETL pipelines
Justify system choices (SQL vs NoSQL etc.)
Design a data ingestion architecture
Explain data cleaning techniques
Discuss data governance and licensing
