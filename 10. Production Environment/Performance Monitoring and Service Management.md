Performance monitoring ensures systems are reliable from the user’s perspective, while service management ensures incidents are handled, learned from, and improved over time.

Instructor Insight (.vtt-enhanced)

A recurring real-world theme from delivery:

“Everything looked fine on dashboards… but users were complaining”

This is why:

Monitoring must focus on user experience, not system metrics

2. Why Reliability is a Feature

From page 8 :

Users care about:
Latency
Freshness
Errors
Applied Explanation

Traditional thinking:

“Server uptime = success”

Modern thinking:

“User gets correct data on time = success”
Key Insight

Reliability is measured in outcomes, not infrastructure

EPA-Level Thinking

“I focus on user-facing metrics such as latency and data freshness to ensure reliability reflects real business impact.”

3. SLIs, SLOs & Error Budgets (CORE EPA CONCEPT)

From page 9 :

SLI → What you measure
SLO → Target level
Error Budget → Acceptable failure
Applied Explanation

Example:

SLI → % of successful pipeline runs
SLO → 99.5% success rate
Error budget → 0.5% failures allowed
Why this matters
Prevents over-engineering
Balances reliability vs delivery speed
.vtt Insight

Common teaching point:

“If you don’t define success, you can’t measure failure”

Key Insight

SLOs align engineering with business expectations

4. Metrics That Actually Matter

From page 10 :

p95 / p99 latency (not averages)
Data freshness
Completeness
Cost per success
Applied Explanation

Why not averages?

Averages hide real issues
Long-tail latency (p95/p99) shows user pain
Example
Average latency = 1s → looks fine
p99 latency = 10s → bad user experience
Key Insight

Measure what users feel, not what systems report

5. Dashboard Design (VERY IMPORTANT)

From page 11 :

Three layers:

Outcomes (SLIs)
Explanations (pipeline stages)
Resources (CPU, memory)
Applied Explanation

Good dashboard:

Shows problem → explains cause → shows root

Bad dashboard:

Shows random metrics with no story
Key Insight

A dashboard should tell one clear story

6. Identifying Bottlenecks (Advanced Skill)

From page 12 :

Latency + CPU → compute issue
Lag + low CPU → downstream issue
Applied Understanding

This is diagnostic thinking:

Don’t fix symptoms
Identify root cause
.vtt Insight

Common real-world mistake:

“Teams fix the wrong bottleneck because they look at one metric in isolation”

Key Insight

Always read signals together

7. Incident Response (CRITICAL EPA AREA)

From page 13 :

First 15 minutes:

Declare incident early
Assign roles
Restore service first
Applied Explanation

This links directly to Module 9:

Stakeholders → communication
Governance → accountability
Key Insight

Fix first, investigate later

.vtt Insight

Real issue often seen:

“No one knew who was in charge → delays, confusion, worse impact”

8. Playbooks & Alerting

From page 14 :

Playbooks = predefined actions
Alerts = actionable signals
Applied Explanation

Bad alert:

Wakes you up → no action

Good alert:

Tells you exactly what to do
Key Insight

Alerts should lead directly to action

9. Post-Incident Reviews (HIGH VALUE)

From page 15 + template :

Structure includes:

Summary (user impact first)
Timeline
Impact (SLO/SLA breach)
Contributing factors
Actions (prevent, contain, detect)
Applied Explanation

This is how organisations improve:

Not blaming people
Fixing systems
Key Insight

Incidents are learning opportunities

EPA-Level Thinking

“I conducted a blameless post-incident review focusing on user impact, root causes, and actionable improvements.”

10. Lab Integration (Automation)

From page 17 :

Automate workflows using Airflow
Applied Understanding

This connects to:

MLOps (automation)
Technical debt (reduce manual work)
Key Insight

Automation improves reliability and reduces human error

11. What This Topic Is REALLY Testing

You are being assessed on your ability to:

Monitor systems effectively
Define meaningful metrics
Respond to incidents
Improve systems continuously
12. KSB Coverage Check (Explicit)
Knowledge (K)
K6 (Performance & reliability)
Understanding monitoring, SLIs, SLOs
K2 (Business impact)
Understanding user-focused metrics
Skills (S)
S4 (Monitoring & evaluation)
Designing dashboards and detecting issues
S5 (System design)
Implementing monitoring and alerting
S8 (Communication)
Incident reporting and stakeholder updates
Behaviours (B)
B1 (Responsibility)
Owning system reliability
B2 (Continuous improvement)
Learning from incidents
B4 (Professionalism)
Structured incident response
13. Distinction-Level EPA Answer (Model Response)
Question:

“How would you monitor and manage the performance of a data pipeline in production?”

Model Answer (Distinction Level)

To monitor and manage the performance of a data pipeline in production, I would implement a structured approach focused on user outcomes, proactive monitoring, and continuous improvement.

Firstly, I would define Service Level Indicators (SLIs) that reflect user experience, such as data freshness, latency, and error rates. I would then establish Service Level Objectives (SLOs) to set clear performance targets, along with error budgets to balance reliability with development velocity.

I would design dashboards that present a clear, layered view of system performance. The top layer would display user-facing outcomes, such as pipeline success rates, while the middle layer would provide explanations such as stage-level latency, and the bottom layer would show infrastructure metrics like CPU and memory usage. This ensures that issues can be quickly identified and diagnosed.

To detect performance issues, I would monitor key metrics such as p95 and p99 latency, as averages can mask user-impacting problems. I would also analyse multiple signals together, such as latency, lag, and resource usage, to accurately identify bottlenecks rather than addressing symptoms.

In the event of an incident, I would follow a structured response process by declaring the incident early, assigning clear roles, and prioritising service restoration. I would use predefined playbooks to guide response actions and ensure consistency under pressure.

After resolving the incident, I would conduct a blameless post-incident review, focusing on user impact, root causes, and contributing factors. I would define actionable improvements categorised into prevention, detection, and containment, ensuring that similar issues are avoided in the future.

Finally, I would continuously refine monitoring and alerting systems to ensure alerts are meaningful and actionable, and automate workflows where possible to improve reliability and reduce human error.

This approach ensures that the pipeline is not only monitored effectively but also continuously improved, aligning technical performance with business and user needs.

Why This Hits Distinction
Covers monitor → detect → respond → improve
Links technical + business + operational thinking
Includes real-world practices (SLOs, dashboards, playbooks)
Demonstrates continuous improvement mindset

14. Final Instructor Insight

At distinction level:

Monitoring is not about collecting metrics — it is about understanding and improving user experience

15. FINAL MODULE 10 BIG PICTURE (EPA GOLD)

You can now explain:

M10T2 → MLOps (deploy + monitor models)
M10T3 → Technical debt (maintain systems)
M10T4 → Monitoring & incidents (operate systems)
Final Understanding

A complete data engineer builds systems, deploys them, maintains them, monitors them, and continuously improves them based on real-world performance
