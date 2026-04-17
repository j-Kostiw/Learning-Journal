Core Theme of This Session

The entire module is about:

Designing data systems that are environmentally sustainable, ethically responsible, and aligned with business strategy

This is not just technical — it combines:

Engineering decisions
Business alignment
Ethics and CSR
2. Key Concepts Recap (From Slides)
Environmental Risks in Data Systems (LO1)

From the recap slides :

What you must understand
Compute intensity = energy consumption
Idle resources = wasted emissions + cost
Cloud region choice = different carbon footprints
Inefficient pipelines = hidden sustainability risk
EPA-Level Insight

A strong answer doesn’t just list issues — it:

Explains why they increase emissions
Links them to cost + scalability trade-offs
KSB Mapping
K1 / K5 – Understanding infrastructure & cloud environments
S3 / S4 – Evaluating system performance and efficiency
B1 – Considering environmental impact in decisions
Sustainable System Design (LO2)

From slides :

Principles to apply
Minimise energy across the entire lifecycle
Use managed services / serverless
Design for carbon efficiency, not just performance
Shared responsibility (cloud provider ≠ full responsibility)
Enhancement (What examiners look for)

You should be able to justify:

Why serverless reduces idle compute
Why autoscaling improves sustainability
Trade-offs (e.g. latency vs efficiency)
KSB Mapping
K7 / K9 – Architecture & system design
S5 / S6 – Designing efficient, scalable pipelines
B2 – Ownership of sustainable design choices
Sustainable Data Management (LO3)

From slides :

Key techniques
Data lifecycle policies (delete, archive)
Cold storage for infrequent access
Compression & partitioning
Avoiding data hoarding
Deeper understanding

Bad data management = hidden emissions:

Storing unused data still consumes energy
Poor partitioning increases query compute
KSB Mapping
K4 / K8 – Data storage & structures
S2 / S7 – Managing and optimising datasets
B1 – Responsible use of data
Ethics & CSR in Data Engineering (LO4–LO6)

From slides :

Core ideas
CSR = more than environment (includes ethics + inclusion)
Align engineering work with organisational sustainability goals
Learn from real-world leaders
What EPA expects
Link technical decisions → business impact
Show awareness of:
Bias
Accessibility
Transparency
KSB Mapping
K10 / K11 – Ethics, governance, regulation
S8 / S9 – Communicating and aligning with stakeholders
B3 / B4 – Professional responsibility and ethical behaviour
3. GreenStack Case Study – What You Should Extract
Business Context

From case study :

GreenStack is trying to balance:

Environmental sustainability
CSR & ethics
Performance & scalability

👉 This is exactly the EPA scenario style.

Current Architecture (Key Weaknesses)

From page 2 :

Multi-region AWS (not optimised)
Hourly ingestion (may be unnecessary frequency)
Nightly Spark jobs on EC2 (high compute)
No lifecycle policies
No emissions tracking
Instructor Insight

This system is:

Functional but not efficient or sustainable
4. Activity Breakdown with Model Answers
Activity 1A – Environmental Risks (LO1)
Strong Answers Should Identify:
Overuse of EC2 clusters → high idle compute
No lifecycle policies → storage sprawl
Hourly ingestion → unnecessary processing
Multi-region without optimisation → higher emissions
KSB Link
S3 – Analyse system performance
K5 – Cloud infrastructure awareness
Activity 1B – Design Improvements (LO2)
High-quality suggestions:
Move EC2 → serverless (Lambda / Glue)
Introduce autoscaling or job scheduling
Use carbon-aware region selection
Optimise ingestion frequency
Advanced (Distinction-level thinking)
Introduce event-driven pipelines
Use spot instances for batch jobs
KSB Link
S5 / S6 – Designing scalable systems
K7 – Architecture design
Activity 1C – Data Management Plan (LO3)
Model structure:
Hot data: recent, frequently accessed
Cold data: archived to cheaper storage
Deletion policy: e.g. delete after 90 days
Governance: assign data owners
Strong answers include:
Automation (lifecycle rules)
Governance roles
Cost + sustainability link
KSB Link
S2 / S7 – Data lifecycle management
B1 – Responsible data handling
5. Activity 2 – CSR & Strategy
2A – CSR Features (LO4)
Good examples:
Emissions dashboards for clients
Accessibility-first UI design
Responsible AI (bias checks, explainability)

From Microsoft case study :

Real-time emissions dashboards are highly valuable
KSB Link
K10 – Ethics
S8 – Stakeholder communication
2B – Internal Strategy (LO5)
Strong answers:
Sustainability training in onboarding
Vendor selection based on ESG
Carbon tracking for teams
Distinction-level:
Introduce KPIs for sustainability
Embed into engineering standards
KSB Link
S9 – Working with stakeholders
B3 – Professional responsibility
2C – Learning from Industry (LO6)
Microsoft (Data-first sustainability)
Build platforms for tracking + reporting emissions
Reusable data models
Google (Carbon-aware computing)
Run workloads when energy is cleanest
Move compute geographically
What examiners want:
Can you transfer ideas, not just describe them?
Example Answer
Google’s carbon-aware scheduling → feasible for GreenStack if:
They have real-time energy data
Automation capability exists
KSB Link
K7 – Applying design patterns
S6 – Adapting solutions
B2 – Innovation mindset
6. Key Takeaways for EPA
1. Always Link Tech → Impact

Not just:

“Use serverless”

But:

“Use serverless to reduce idle compute, lowering energy consumption and cost”

2. Think in Trade-offs
Performance vs sustainability
Cost vs scalability
Speed vs efficiency
3. Use Structured Answers

For case questions:

Identify problem
Explain impact
Propose solution
Justify with framework
4. Use Real-World References

Mention:

AWS Sustainability Pillar
Green Software Foundation
Microsoft / Google examples
7. Final Reflection (What Makes a Strong Apprentice)

A strong Level 5 Data Engineer:

Designs systems efficiently AND responsibly
Understands business + environmental impact
Can justify decisions clearly
[L5DE M11T3 - Re-cap of sustainability considerations.pdf](https://github.com/user-attachments/files/26818047/L5DE.M11T3.-.Re-cap.of.sustainability.considerations.pdf)
