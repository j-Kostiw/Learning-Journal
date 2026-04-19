Understanding, managing, and mitigating risks in data ingestion systems

At EPA level, this is about:

Identifying risks
Explaining impact
Proposing mitigation strategies
2. Why Data Ingestion Risk Matters

From case study (page 3) :

Example: Facebook (Meta)
Ingests data from:
User interactions
Posts
External sites
Key approach:
Uses SLAs (Service Level Agreements) to manage risk
Impact:
Ensures data quality
Maintains security
Supports compliance
Builds user trust
Instructor Insight

At EPA level, always link:

Risk → Business impact → Mitigation

3. Service Level Agreements (SLAs)
What are SLAs?

Defined expectations for system performance and reliability

Why they matter

From knowledge check (page 4) :

Ensure timely data ingestion
Define acceptable performance
Provide escalation paths
Example SLA metrics:
Data latency (e.g. <5 minutes delay)
Data quality thresholds
System uptime
KSB Mapping
K6 – System reliability
S4 – Monitoring and evaluation
B2 – Accountability
4. Common Data Ingestion Risks

From page 8 :

Key Risks You MUST Know
1. System Failures
Pipelines crash or stop working
2. Performance Issues
Systems slow or inefficient
3. Security Vulnerabilities
Exposure to attacks (e.g. SQL injection)
4. Data Quality Issues
Inconsistent, missing, or incorrect data
5. PII Mismanagement
Sensitive data handled incorrectly
6. Storage & Cost Issues
Unused data building up
7. Changing Requirements
Frequency or volume changes
8. Schema Changes
Breaking downstream systems
EPA Insight

Strong answers:

Identify multiple risks
Explain consequences
Suggest mitigation
5. Troubleshooting & Risk Mitigation

From “Lessons learned” (page 10) :

Key practices:
Testing and code reviews
Documenting failures
Asking for help
Reflecting on fixes
Instructor Insight

Good engineers:

Learn from failures and prevent recurrence

KSB Mapping
S5 – Problem solving
B2 – Continuous improvement
6. Root Cause Analysis (CRITICAL FOR EPA)

From page 11 :

Steps:
Identify contributing factors
Organise events (timeline)
Classify causes
Identify root cause
The “5 Whys” Technique (Page 12)

Example:

Problem → ask “why?” repeatedly
Leads to root cause
EPA Tip

Always go beyond:

“The system failed”

Instead:

“The system failed due to upstream schema changes not being validated”

KSB Mapping
S4 – Evaluation
K6 – Problem analysis
7. Sustainability & Data Risks

From page 13 :

Key Risks:
Poor pipeline design
Lack of monitoring
No automation
Excess data storage
No compression
Why it matters:

Poor data design = higher energy usage and cost

Example:
Storing unused data increases:
Storage cost
Carbon footprint
KSB Mapping
B1 – Responsible practice
K7 – Sustainable systems
8. Cybersecurity Risks in Ingestion

From page 15 :

Example: SQL Injection
Malicious input manipulates queries
Can expose entire database
Mitigation:
Input validation
Parameterised queries
Authentication controls
EPA Insight

Security must always be included in ingestion design

KSB Mapping
K10 – Security
S2 – Secure data handling
9. Data Quality Improvement

From diagram (page 16) :

Lifecycle:
Assess data quality
Identify root causes
Implement improvements
Monitor results
Key idea:

Data quality is continuous, not one-off

10. Unused Data & Archiving

From page 17 :

Risks:
Slower systems
Higher storage costs
Compliance issues
Solution:
Data lifecycle policies
Archiving strategies
Deletion rules
EPA Insight

Mention:

“Data minimisation” (important keyword)

11. Risk Register & Reporting

From pages 18–19 :

Risk Register Includes:
Risk description
Likelihood
Impact
Mitigation strategy
Risk Reporting:
Ongoing monitoring
Communication to stakeholders
EPA Tip

Always show:

Structured risk management approach

KSB Mapping
S8 – Communication
S4 – Monitoring
12. Handling PII & Sensitive Data

From objectives (page 5) :

Key strategies:
Encryption
Access control
Data masking
Compliance (GDPR etc.)
Why it matters:
Legal requirements
Ethical responsibility
KSB Mapping
K10 – Governance
B1 – Ethics
13. What Examiners Are Looking For
1. Risk Awareness

You must identify:

Technical risks
Business risks
Security risks
2. Mitigation Thinking

Always include:

Risk → Solution

3. Structured Answers

Use:

Identify
Explain
Mitigate
4. Real-World Thinking

Reference:

SLAs
Monitoring
Governance
14. Final Takeaways

From summary (page 22) :

SLAs ensure reliability and quality
Risks must be monitored and managed
PII handling is critical
Data quality must be continuously improved
Sustainable design reduces impact
15. EPA Revision Checklist

You should be able to:

Define and explain SLAs
Identify data ingestion risks
Perform root cause analysis
Suggest risk mitigation strategies
Explain data quality improvement
Discuss security and PII handling
Describe risk registers and reporting
16. Final Instructor Insight

A distinction-level apprentice doesn’t just build pipelines — they:

Anticipate risks, design safeguards, and continuously improve system reliability
