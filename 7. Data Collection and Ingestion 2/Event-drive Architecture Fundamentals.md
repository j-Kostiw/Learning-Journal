Event-Driven Architecture (EDA) enables real-time, scalable data systems by reacting to events as they occur rather than processing data in batches.

From the opening slides :

85% of organisations already use EDA
94% plan to expand its use
Instructor Insight

This tells you:

EDA is industry standard
You are expected to understand it conceptually AND architecturally
2. Why Event-Driven Architecture Exists

From “evolution of data processing” (page 5) :

Full Explanation (EPA Style)

Traditional batch systems struggle because modern data is:

High volume
High velocity
Constantly changing

Event-driven systems solve this by:

Processing data as it is created, enabling real-time decision-making.

Key Points
Data volumes are growing exponentially
Batch processing introduces delays
Real-time systems provide immediate insights
EDA supports dynamic, scalable systems
KSB Mapping
K7 / K20 – Understanding modern data architectures
S3 / S5 – Designing scalable pipelines
B2 – Adapting to modern technologies
3. Real-World Case Study – Tesco

From page 2 :

Explanation

Tesco moved from batch → event-driven using Apache Kafka to solve inventory challenges.

What changed?

Before:

Batch updates → delays
Poor inventory visibility

After:

Real-time updates
Improved supply chain
Better customer experience
Instructor Insight

This is a classic EPA example:

Business problem → Technical solution → Measurable impact

KSB Mapping
K2 – Business requirements
S8 – Linking tech to business value
B1 – Outcome-focused thinking
4. Fundamentals of Event-Driven Architecture

From page 6 :

Full Explanation

Event-driven architecture is a design paradigm where systems communicate through events instead of direct requests.

This means:

Systems don’t wait for responses
They react when something happens
Key Components
Events → Something that happened (e.g. purchase)
Producers → Generate events
Consumers → React to events
Brokers → Route events between systems
Critical Concept: Asynchronous Communication

Systems operate independently and do not need to wait for each other

Why this matters:
Improves scalability
Reduces system dependencies
Enables real-time processing
KSB Mapping
K20 / K22 – Architecture design
S12 / S13 – System modelling
B2 – Efficient system thinking
5. Publish-Subscribe (Pub-Sub) Model

From page 8 :

Full Explanation

The pub-sub model allows systems to communicate via messages without direct connections.

How it works:
Publishers send messages to topics
Subscribers listen to topics
No direct link between them
Key Advantage: Decoupling

Systems can evolve independently without breaking each other

Example (from slide):
Stock market feeds
Publishers → price updates
Subscribers → trading systems
EPA Insight

Strong answers include:

“Pub-sub decouples producers and consumers, improving scalability and flexibility”

KSB Mapping
K20 / K24 – Distributed systems
S2 / S12 – Data flow design
B4 – Best practice design thinking
6. Introduction to Kafka

From page 9 :

Full Explanation

Apache Kafka is a distributed event streaming platform used to handle real-time data pipelines.

Core Components
Topics → Categories of data
Partitions → Enable parallel processing
Producers → Send data
Consumers → Read data
Consumer Groups → Distribute workload
Why Kafka is important
Handles large-scale real-time data
Ensures fault tolerance
Enables scalable pipelines
KSB Mapping
K7 / K25 – Tools and platforms
S5 / S13 – Pipeline implementation
B2 – Scalable thinking
7. Kafka Clusters & Data Consistency

From page 10 :

Explanation

Kafka ensures reliability through:

Clusters → Multiple brokers
Replication → Copies of data
Leader/Follower model
Why this matters

Ensures systems remain available even if components fail

Key Points
Horizontal scaling
Fault tolerance
Strong consistency
KSB Mapping
K20 / K22 – Distributed architecture
S13 / S14 – Designing resilient systems
8. Kafka as a Log (CRITICAL CONCEPT)

From page 11 :

Full Explanation

Kafka stores data as an immutable log, where events are appended and never changed.

Key Concepts
Messages stored sequentially
Each message has an offset
Consumers track their own position
Why this is powerful
Enables replay of data
Supports large-scale processing
Improves reliability
EPA Insight

This is a distinction-level concept:

“Kafka’s log-based design allows systems to replay and reprocess events, improving fault tolerance and auditability”

KSB Mapping
K20 / K26 – Advanced architecture
S12 / S13 – System design
9. Challenges in Kafka / EDA

From page 12 :

Common Issues
Zookeeper coordination
Network configuration
Resource allocation
Security setup
Instructor Insight

EDA is powerful but:

More complex to implement and manage

KSB Mapping
S5 – Problem solving
B2 – Continuous improvement
10. Industry Relevance of EDA

From page 7 :

Where EDA is used:
Healthcare → patient monitoring
Retail → inventory updates
Transport → real-time tracking
Key idea:

EDA enables real-time business operations across industries

11. Collaboration & Professional Skills

From page 13 :

Key practices:
Clear communication (Slack, Teams)
Documentation (GitHub, Confluence)
Defined roles
Agile working
KSB Mapping
S8 / S9 – Communication
B4 / B5 – Teamwork
12. What Examiners Are Looking For
1. Real-Time Thinking

Not:

“Process data”

But:

“Process data as events occur”

2. Architecture Understanding

Explain:

Components
Flow
Benefits
3. Trade-offs

EDA:

✔ Scalable
✔ Real-time
✖ More complex
4. Business Alignment

Always link:

Architecture → Business outcome

13. Final Takeaways

From summary (page 16) :

EDA enables asynchronous, scalable systems
Pub-sub enables decoupled communication
Kafka supports real-time pipelines
Log-based design improves reliability
Clusters ensure fault tolerance
14. EPA Revision Checklist

You should be able to:

Explain event-driven architecture clearly
Describe pub-sub model
Explain Kafka components
Justify real-time vs batch systems
Discuss scalability and fault tolerance
Link EDA to business value
15. Final Instructor Insight

A distinction-level apprentice:

Thinks in events, not processes — designing systems that react in real-time, scale independently, and deliver immediate business value
