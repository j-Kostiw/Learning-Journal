From Data Pipelines to Data Architectures
1. Core Theme of This Topic

This topic is about moving from building pipelines to designing full data architectures that scale, perform, and deliver business value.

From the session intro :

You are no longer just:

Moving data from A → B

You are now expected to:

Design systems that handle growth, complexity, and real-world constraints
Instructor Insight

At EPA level, this is a mindset shift:

A pipeline is a component — an architecture is the whole system

2. Real-World Framing – Zalando Case Study

From page 3 :

Zalando processes:

Billions of daily events
Real-time recommendations
High traffic spikes (e.g. Black Friday)

They solved this using:

Kafka + Kinesis → real-time ingestion
AWS Lambda → scalable compute
Airflow → orchestration
S3 + Redshift → scalable storage
What this teaches you

This is not just tooling — it’s architecture thinking:

Different components solve different problems, but must work together cohesively

EPA-Level Understanding

A strong answer would say:

“Zalando uses a modular, event-driven architecture to decouple ingestion, processing, and storage, enabling real-time scalability and resilience during peak demand.”

3. What is Scalability? (Core Concept)

From page 8 :

Scalability is the ability of a system to handle increasing data volume, users, and complexity without performance loss.

Applied Understanding

Scalability is not just about “handling more data” — it is about:

Maintaining performance under load
Controlling cost as systems grow
Ensuring reliability at scale
Practical Example
Small system → runs on one machine
Scaled system → distributed across many nodes
Instructor Insight

At EPA level:

You must explain scalability in terms of performance + reliability + cost

4. Scaling Data Pipelines (How It’s Done)

From diagrams on page 9 :

You are shown:

Vertical vs horizontal scaling
Batch vs streaming pipelines
MapReduce-style distributed processing
Applied Explanation
Vertical Scaling
Increase power of one machine
Limited and expensive
Horizontal Scaling
Add more machines
More flexible and scalable
Batch vs Streaming
Batch → efficient but delayed
Streaming → real-time but complex
Instructor Insight

A strong apprentice doesn’t just describe these — they choose:

“Streaming is used where real-time decisions are required; batch is used for cost-efficient large-scale processing.”

5. Tools for Scalable Pipelines

From page 10 :

Spark → distributed processing
Kafka → real-time streaming
Airflow/Prefect → orchestration
Applied Understanding

These tools map directly to architecture layers:

Layer	Tool
Ingestion	Kafka
Processing	Spark
Orchestration	Airflow
Instructor Insight

EPA answers should show:

You understand how tools fit together, not just what they do

6. Ensuring Performance

From page 11 :

Performance depends on:

Throughput (how much data processed)
Latency (how fast data is processed)
Resource usage
Applied Explanation

Performance tuning involves:

Optimising transformations
Choosing efficient storage formats
Monitoring system metrics
Key Insight

You cannot scale what you cannot measure

7. Building for Reliability

From page 12 :

Reliable systems are designed to handle failure gracefully

Applied Techniques
Retry logic
Checkpointing
Idempotent processing
Decoupling with Kafka
Real Understanding

Failure is expected in distributed systems:

Good systems recover automatically without data loss

EPA-Level Thinking

A strong answer explains:

“Fault tolerance ensures that failures do not disrupt pipeline execution or corrupt data integrity.”

8. Designing Scalable Architectures

From page 13 :

Full Explanation

Scalable architectures are modular, loosely coupled, and often event-driven.

What this means in practice
Break systems into independent components
Allow each component to scale separately
Use messaging systems (Kafka) to connect them
Instructor Insight

This is one of the most important distinctions:

Monolithic systems break at scale — modular systems grow

9. Architecture Patterns (VERY IMPORTANT)
Lambda Architecture (Page 14)
Batch layer + real-time layer
Provides both accuracy and speed
Kappa Architecture (Page 15)
Stream-only processing
Simpler but requires strong streaming capability
Lakehouse Architecture (Page 16)
Combines data lake + warehouse
Supports analytics + ML
Applied Understanding

You must justify choice:

Lambda → complex but powerful
Kappa → simpler, real-time focus
Lakehouse → unified analytics
Instructor Insight

EPA answers should include:

“The choice of architecture depends on trade-offs between complexity, latency, and data requirements.”

10. Cost vs Performance Trade-Offs

From page 17 :

Full Explanation

Scalability is not just technical — it is economic

Applied Examples
Cold data → cheap storage
Hot data → fast access storage
Batch jobs → reduce compute costs
Key Insight

Over-engineering = wasted cost
Under-engineering = system failure

11. What This Topic Is Really Testing

This topic brings everything together:

You must be able to:

Design systems end-to-end
Balance trade-offs
Justify decisions
12. KSB Application Summary (What You Can Now DO)

This is the key improvement you asked for — linking learning → KSB application.

Knowledge (K)

You now demonstrate:

K7 / K8 (Architecture & Systems)
You can explain how distributed systems scale and why modular design is required.
K20+ (Modern Architectures)
You understand event-driven, streaming, and hybrid architectures like Lambda and Kappa.
Skills (S)

You can now:

S2 / S3 (Data Processing & Pipelines)
Design pipelines that scale using streaming, partitioning, and orchestration.
S12 / S13 (Architecture Design)
Design full systems, not just pipelines, including ingestion, processing, and storage layers.
S14 / S15 (Optimisation)
Make decisions that balance performance, cost, and reliability.
Behaviours (B)

You demonstrate:

B1 (Responsibility)
You consider cost, performance, and reliability impacts of your designs.
B2 (Continuous Improvement)
You monitor, optimise, and evolve systems over time.
B4 (Best Practice Thinking)
You design modular, scalable, and maintainable architectures.
13. Final Instructor Insight (Key Takeaway)

A distinction-level apprentice doesn’t just build pipelines — they:

Design scalable, reliable, and cost-efficient data architectures that evolve with business needs
