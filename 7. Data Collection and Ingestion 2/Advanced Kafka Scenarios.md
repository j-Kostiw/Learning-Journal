This topic moves from understanding Kafka → to applying it in real-world, enterprise scenarios including cloud integration, security, and troubleshooting.

From the introduction :

81% of companies use Kafka for pipelines
66% use it for stream processing
Instructor Insight

You are now expected to:

Go beyond “what Kafka is”
Explain how to operate, secure, and troubleshoot it in production
2. Real-World Case Study – Audi (Predictive Maintenance)

From page 2 :

Full Explanation

Audi uses Kafka to:

Continuously monitor vehicle sensor data and predict failures in real time.

Business Impact
Reduced maintenance costs
Improved reliability
Increased customer satisfaction
Instructor Insight

This is a high-quality EPA example:

Real-time data → predictive insight → business value

KSB Mapping
K2 – Business context
S8 – Linking data solutions to outcomes
B1 – Value-driven thinking
3. Cloud-Based Event Streaming Services

From page 5 :

Full Explanation

Modern architectures increasingly use:

Managed cloud services instead of self-managed Kafka clusters

Key Platforms
Azure
AWS
Google Cloud
Benefits
Managed infrastructure
Easier scaling
Integration with cloud ecosystems
Instructor Insight

You must justify:

When to use Kafka vs managed services

KSB Mapping
K7 / K25 – Cloud platforms
S5 – Tool selection
B2 – Adaptability
4. Azure Event Hubs vs Event Grid

From page 6 :

Full Explanation

These are two different types of event services:

Event Hubs
Real-time ingestion
Similar to Kafka
Used for big data pipelines
Event Grid
Event routing service
Used for triggering workflows
Key Difference

Event Hubs = data streaming
Event Grid = event routing

Instructor Insight

Strong EPA answers:

Clearly distinguish ingestion vs routing systems

KSB Mapping
K20 / K22 – Architecture understanding
S12 – System design
5. Kafka vs Azure Event Hubs

From comparison (page 7) :

Key Differences
Kafka
Self-managed
Full control
Complex setup
Event Hubs
Fully managed
Easier to use
Less control
EPA-Level Insight

Kafka = flexibility
Event Hubs = simplicity

When to use each
Kafka → custom, complex systems
Event Hubs → cloud-native solutions
KSB Mapping
K7 – Technology comparison
S5 / S6 – Choosing solutions
6. AWS & GCP Alternatives

From page 8 :

Key Services
AWS:
Kinesis → streaming
SNS → pub-sub
SQS → messaging queue
GCP:
Pub/Sub → global messaging
Instructor Insight

You should recognise:

Kafka concepts exist across all cloud platforms

KSB Mapping
K7 / K25 – Multi-cloud awareness
S6 – Applying knowledge
7. Industry Use Cases (VERY IMPORTANT)

From page 9 :

Examples
Financial Services
Fraud detection in real time
E-commerce
Personalised recommendations
IoT / Manufacturing
Predictive maintenance
EPA Insight

Always link:

Use case → data → value

8. Kafka Security (CRITICAL FOR EPA)
SSL / TLS (Page 10)
Full Explanation

Encrypts data in transit to prevent interception

Why it matters:
Protects sensitive data
Ensures compliance (GDPR, HIPAA)
Prevents internal threats
SASL (Page 11)
Full Explanation

Provides authentication (who can access the system)

Mechanisms:
Kerberos
SCRAM
OAuth
ACL (Page 12)
Full Explanation

Controls authorisation (what users can do)

Key idea:

Authentication ≠ Authorisation

Instructor Insight

A strong answer explains:

SSL = encryption
SASL = authentication
ACL = authorisation

KSB Mapping
K10 – Security & governance
S2 – Secure data handling
B1 – Ethical responsibility
9. Troubleshooting Kafka Systems

From pages 13–14 :

Common Issues You MUST Know
1. Consumer Lag
Messages processed too slowly
2. Broker Failure
System crashes or unavailable
3. Under-replicated Partitions
Data not fully replicated
4. Message Loss
Missing or inconsistent data
5. High Latency
Delays in processing
Instructor Insight

For EPA:

Always explain:

Symptom
Cause
Solution
Example (Distinction Level)

Issue: Consumer lag
Cause: Not enough consumers
Solution: Scale consumer group

KSB Mapping
S4 / S5 – Problem solving
K6 – System behaviour
10. Root Cause Analysis (CRITICAL SKILL)

From page 15 :

Techniques
1. 5 Whys
Ask “why” repeatedly
2. Fishbone Diagram
Categorise causes
3. Fault Tree Analysis
Logical breakdown of failures
Instructor Insight

EPA answers must:

Go beyond symptoms → identify root cause

KSB Mapping
S4 – Evaluation
B2 – Continuous improvement
11. Knowledge Check Scenario (Important)

From page 3 :

Scenario:

Delayed sensor data in Kafka system

Model Answer Approach
Step 1 – Identify symptoms
Data delays
Inaccurate predictions
Step 2 – Analyse causes
Consumer lag
Network issues
Broker overload
Step 3 – Implement solutions
Scale consumers
Optimise processing
Check infrastructure
Step 4 – Prevent
Monitoring
Alerts
Autoscaling
12. What Examiners Are Looking For
1. Real-World Application

Not:

“Kafka processes data”

But:

“Kafka enables real-time analytics and predictive insights”

2. Security Awareness

You must include:

Encryption
Authentication
Access control
3. Troubleshooting Thinking

Always structure:

Problem → Cause → Solution
4. Tool Comparison

Explain:

Kafka vs cloud alternatives
13. Final Takeaways

From summary (page 17) :

Event streaming is critical in modern systems
Cloud services simplify Kafka usage
Security is essential (SSL, SASL, ACL)
Common issues must be understood
Root cause analysis is key
14. EPA Revision Checklist

You should be able to:

Compare Kafka vs cloud services
Explain Event Hubs vs Event Grid
Describe Kafka security (SSL, SASL, ACL)
Identify and fix Kafka issues
Apply root cause analysis techniques
Link Kafka to business use cases
15. Final Instructor Insight

A distinction-level apprentice:

Does not just build streaming systems — they secure, scale, troubleshoot, and justify them in real-world business contexts
