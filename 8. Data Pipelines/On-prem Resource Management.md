On-premise resource management is about designing, maintaining, and optimising physical infrastructure to support reliable and efficient data pipelines.

From the session overview :

You are expected to:

Design and maintain infrastructure
Optimise resource usage
Build scalable and reliable on-prem workflows
Instructor Insight

This topic shifts your thinking from:

“Using cloud resources” → “owning the entire system stack”

2. Why On-Prem Resource Management Matters
Real-World Case – Haribo ERP Failure

From page 3 :

Full Explanation

Haribo implemented an ERP system but failed due to:

Poor process mapping
No infrastructure stress testing
No load balancing or monitoring
Business Impact
Inventory failures → empty shelves
Sales dropped by 25%
Instructor Insight

At EPA level:

Poor infrastructure management = direct financial loss

KSB Mapping
K2 – Business impact
S5 – System reliability
B1 – Responsibility
3. What is On-Premise Infrastructure?

From page 8 :

Full Explanation

On-premise infrastructure consists of physical servers, storage, and networking systems that are fully managed by the organisation.

Key Characteristics
Physical hardware (servers, disks, networking)
Self-managed environment
No automatic scaling
Key Difference vs Cloud
On-Prem	Cloud
Manual setup	Managed services
Fixed capacity	Elastic scaling
Full control	Abstracted infrastructure
Instructor Insight

On-prem requires systems engineering thinking, not just coding

KSB Mapping
K7 / K8 – Infrastructure and systems
S12 – Architecture understanding
4. Setting Up Infrastructure (Design Phase)

From page 9 :

Full Explanation

Proper infrastructure setup ensures systems are secure, scalable, and resilient from the start.

Key Considerations
Compute, storage, and redundancy planning
Secure network topology
OS and runtime hardening
From diagram (page 9)

The diagram highlights:

Capacity planning
Security configuration
Network design
Instructor Insight

Poor setup decisions are difficult and costly to fix later

KSB Mapping
S12 / S13 – System design
K6 – Infrastructure planning
5. Maintenance & System Health

From page 10 :

Full Explanation

Ongoing maintenance ensures systems remain secure, stable, and performant.

Key Practices
Regular patching and updates
Monitor CPU, memory, disk
Test backups and recovery
Instructor Insight

Maintenance is continuous, not reactive

KSB Mapping
S4 – Monitoring
B2 – Continuous improvement
6. Resource Awareness (CRITICAL CONCEPT)

From page 11 :

Full Explanation

On-prem systems have finite resources, so efficient usage is critical.

Key Resources
CPU
RAM
Disk I/O
Network bandwidth
Key Limitation

There is NO “scale-up button”

Instructor Insight

Strong EPA answer:

“Unlike cloud systems, on-prem environments require careful capacity planning due to fixed resources”

KSB Mapping
K7 – System constraints
S5 – Resource optimisation
7. Optimising Resource Usage

From page 12 :

Full Explanation

Efficient resource usage ensures pipelines run smoothly without overloading systems.

Key Techniques
Chunk large datasets
Use vectorised operations
Avoid unnecessary I/O
Why this matters
Reduces CPU load
Improves memory efficiency
Prevents bottlenecks
Instructor Insight

Small optimisations = big performance gains

KSB Mapping
S14 / S15 – Optimisation
K7 – Performance
8. Scheduling Strategy (VERY IMPORTANT)

From page 13 :

Full Explanation

Job scheduling ensures workloads are distributed efficiently across limited resources.

Best Practices
Stagger job start times
Prioritise critical workloads
Use off-peak execution
Analogy (from slide)

System = shared kitchen
Jobs = people cooking

Instructor Insight

Poor scheduling causes system crashes even if code is correct

KSB Mapping
S5 – Pipeline management
K6 – System performance
9. Docker & Kubernetes On-Prem

From page 14 :

Full Explanation

Containerisation tools can be used on-prem, but require full manual management.

Key Challenges
Manual provisioning
Network configuration
Storage setup
Monitoring responsibility
Instructor Insight

On-prem Kubernetes = cloud complexity without cloud convenience

KSB Mapping
K7 / K25 – Tools and platforms
S12 – System design
10. Real-World Lessons

From page 15 :

Examples
Manufacturing → staggered jobs prevented failures
Hospital → rehearsed updates enabled safe deployments
University → resource quotas improved fairness
Instructor Insight

Resource management is about fairness, stability, and planning

11. Practical Application (EPA-Level Thinking)

From exercise (page 17) :

Scenario
Add US data to pipeline
Update schema
Rebuild pipeline
What this tests
Scalability
Resource planning
Workflow redesign
Instructor Insight

More data sources = more resource pressure

12. What Examiners Are Looking For
1. Systems Thinking

You must explain:

Infrastructure
Resource limits
Trade-offs
2. Optimisation Awareness

Include:

Efficient processing
Scheduling strategies
3. Reliability Thinking

Explain:

Monitoring
Maintenance
Backups
4. Cloud vs On-Prem Comparison

Strong answers include:

Differences in scalability, cost, and control

13. Final Takeaways

From summary (page 18) :

On-prem systems require full ownership
Resource limits must be managed carefully
Optimisation improves stability
Scheduling prevents overload
Containers still require manual setup
Success comes from planning and monitoring
14. EPA Revision Checklist

You should be able to:

Define on-prem infrastructure
Explain resource constraints
Describe optimisation techniques
Explain scheduling strategies
Compare on-prem vs cloud
Discuss Docker/Kubernetes on-prem
Explain maintenance and monitoring
15. Final Instructor Insight

A distinction-level apprentice:

Thinks like a systems engineer — balancing performance, capacity, and reliability across the entire infrastructure stack
