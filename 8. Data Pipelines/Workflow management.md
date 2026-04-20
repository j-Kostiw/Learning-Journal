Workflow management ensures that data pipelines run reliably, efficiently, and in the correct order by coordinating tasks, dependencies, and automation.

From the session overview :

You are expected to:

Design workflows
Use orchestration tools
Automate and optimise pipelines
Monitor and maintain workflow health
Instructor Insight

This topic is about moving from:

“writing scripts” → “engineering production-grade pipelines”

2. Why Workflow Management Matters

From case study (page 3) :

Full Explanation

Poor workflow management leads to:

Missed runs → outdated data
Failed jobs → blocked pipelines
Poor scheduling → system overload
Real-World Example
Colonial Pipeline outage → $4.4M loss
Caused by lack of workflow resilience
Instructor Insight

At EPA level:

Workflow failures = business failures

KSB Mapping
K2 – Business impact
S5 – Pipeline reliability
B1 – Responsibility
3. What is a Data Workflow?

From page 8 :

Full Explanation

A data workflow is a structured sequence of dependent tasks that move and transform data.

Key Characteristics
Sequence of tasks
Dependencies between tasks
Requires control and visibility
From the diagram (page 8)

The workflow shows:

Data flowing through stages
Tasks connected logically
Transformation at each stage
Instructor Insight

A workflow is NOT just code — it is task coordination and control

KSB Mapping
K4 – Data processing concepts
S2 / S3 – Data pipeline design
4. Core Principles of Workflow Management

From diagram (page 9) :

The 5 Principles
Define task boundaries clearly
Use dependency-driven execution
Design for failure
Centralise logging and monitoring
Keep workflows modular
Full Explanation

Good workflows:

Are easy to debug
Can recover from failure
Scale effectively
Instructor Insight

“Design for failure” is a distinction-level concept

KSB Mapping
K6 / K7 – System design
S12 / S13 – Architecture thinking
B2 – Best practice mindset
5. From Script to Pipeline

From page 10 :

Full Explanation

A pipeline is a coordinated set of tasks, not just a script.

Key Concepts
Tasks have dependencies
Execution order matters
Relationships define structure
Example Flow
Extract → Clean → Summarise → Load
Instructor Insight

Weak answer:

“Run script”

Strong answer:

“Define task dependencies and orchestrate execution”

KSB Mapping
S5 – Pipeline building
K4 – Data transformation
6. Workflow Patterns (VERY IMPORTANT)

From page 11 :

Key Patterns
1. Linear Chain
A → B → C
Simple pipelines
2. Fan-out / Fan-in
Split into parallel tasks
Merge results
3. Conditional Branching
Different paths based on logic
4. Sensor-Driven
Wait for external trigger
Instructor Insight

EPA questions often ask:

“Design a workflow” → you must choose the correct pattern

KSB Mapping
S12 – Workflow design
K7 – Architecture patterns
7. Orchestration Tools – Airflow vs Prefect

From page 12 :

Apache Airflow
Uses DAGs (Directed Acyclic Graphs)
Strong for batch processing
Industry standard
Prefect
Python-native
Easier to use
Better for dynamic workflows
Key Comparison Insight
Tool	Strength
Airflow	Mature, widely used
Prefect	Flexible, modern
Instructor Insight

At EPA level:

You must justify tool choice

KSB Mapping
K7 / K25 – Tools
S5 / S6 – Technology selection
8. Optimising Workflows

From page 13 :

Key Techniques
Parallelism & concurrency
Caching intermediate results
Resource scaling
From diagram (page 13)
Parallel execution speeds up pipelines
Caching avoids repeated work
Instructor Insight

Optimisation = performance + cost efficiency

KSB Mapping
S14 / S15 – Optimisation
K7 – Performance concepts
9. Automating Repetitive Tasks

From page 14 :

Full Explanation

Automation reduces manual work and improves consistency.

What to automate
Scheduled jobs
Event-driven triggers
Reusable workflows
Good Practice
Version control (Git)
Documentation
Modular design
Instructor Insight

Automation is essential for scaling pipelines

KSB Mapping
S5 – Pipeline automation
B2 – Efficiency mindset
10. Monitoring and Maintenance

From page 15 :

What to Monitor
Task success/failure rates
Execution times
Resource usage
Queue backlogs
Key Analogy (from slide)

Pipeline = train system
Tasks = trains
Orchestrator = control tower

Instructor Insight

This links directly to Module 7 monitoring topic

KSB Mapping
S4 – Monitoring
K6 – System performance
11. Maintaining Workflow Health

From page 16 :

Best Practices
Review logs regularly
Set alerts and thresholds
Test changes in isolation
Clean and optimise pipelines
Instructor Insight

Maintenance is ongoing, not one-off

KSB Mapping
S4 / S5 – Monitoring and improvement
B2 – Continuous improvement
12. Practical Application (Important for EPA)

From exercise (page 18) :

Scenario
Integrate UK + French data
Update schema
Rebuild pipeline
What this tests
Handling multiple data sources
Schema evolution
Workflow redesign
Instructor Insight

This is real EPA-style thinking:

Adapt pipelines to new requirements

13. What Examiners Are Looking For
1. Structured Workflow Thinking

You must explain:

Tasks
Dependencies
Execution order
2. Tool Awareness

Mention:

Airflow / Prefect
DAGs
Scheduling
3. Optimisation & Automation

Explain:

Parallel processing
Caching
Triggers
4. Reliability & Monitoring

Include:

Alerts
Logs
Performance tracking
14. Final Takeaways

From summary (page 19) :

Workflows manage data movement
Orchestration tools automate pipelines
Optimisation improves performance
Automation reduces manual effort
Monitoring ensures reliability
15. EPA Revision Checklist

You should be able to:

Define data workflows clearly
Explain workflow principles
Describe workflow patterns
Compare Airflow vs Prefect
Explain optimisation techniques
Describe automation strategies
Explain monitoring and maintenance
16. Final Instructor Insight

A distinction-level apprentice:

Designs workflows that are structured, automated, scalable, and resilient — not just functional
