Technical debt and maintenance focus on ensuring systems remain scalable, reliable, and maintainable over time, rather than degrading due to shortcuts and complexity.

From the objectives :

You must:

Understand technical debt
Measure and prioritise it
Apply maintenance strategies
Manage long-term system health
Instructor Insight (.vtt-enhanced)

A recurring teaching theme:

“Systems don’t fail because of one bug — they fail because of accumulated decisions over time”

This is exactly what technical debt represents.

2. Real-World Case – TSB Migration Failure

From page 3 :

1.3 billion records migrated
System failure → customers locked out
Root causes:
Legacy complexity
Weak testing
Poor governance
Applied Explanation

This is not just a migration issue — it is:

Technical debt (legacy systems)
Testing failure (Module 8)
Governance failure (Module 9)
Business Impact
£48M+ fines
CEO resignation
Months of disruption
Key Insight

Technical debt becomes visible only when systems are stressed

EPA-Level Thinking

“The TSB failure demonstrates how unmanaged technical debt, combined with poor testing and governance, can lead to large-scale system failure.”

3. What is Technical Debt?

From page 8 :

Shortcuts today = complexity tomorrow

Applied Explanation

Technical debt occurs when:

You prioritise speed over quality
You defer proper design
You accumulate complexity
Types of Debt (from page 10)
Code
Infrastructure
Documentation
Architecture
Process
Real Example (from slide)

A batch pipeline adapted for real-time without redesign → instability

.vtt Insight

Often described as:

“Quick fixes that become permanent problems”

Key Insight

Debt is not bad — unmanaged debt is

4. Why Systems Become Complex (Lehman’s Laws)

From page 9 :

Systems must evolve
Complexity increases over time
Without management → systems degrade
Applied Explanation

This explains why:

Pipelines become harder to maintain
Models become harder to update
Systems become fragile
Key Insight

Complexity is inevitable — control is optional

5. Measuring Technical Debt (CRITICAL SKILL)

From page 11 :

Quantitative:
Code complexity
Test coverage
Qualitative:
Developer feedback
Onboarding difficulty
Applied Understanding

You cannot fix what you cannot measure:

High complexity → harder to maintain
Low test coverage → higher risk
Key Insight

Debt must be visible to be manageable

EPA-Level Thinking

“I used metrics such as test coverage and code complexity alongside developer feedback to identify and quantify technical debt.”

6. Prioritising Technical Debt

From page 12 :

Use:

Impact vs Effort matrix
Business risk
Maintenance burden
Applied Explanation

Not all debt should be fixed immediately:

High impact + low effort → quick wins
High impact + high effort → strategic fixes
Key Insight

Technical decisions must align with business priorities

7. Managing Technical Debt (Practical Strategies)

From page 13 :

Refactoring
Quality gates
Documentation
Applied Understanding

This connects directly to previous modules:

Testing (Module 8) → quality gates
CI/CD (MLOps) → automation
Governance (Module 9) → standards
.vtt Insight

A key teaching point:

“If you don’t schedule time to fix debt, it will schedule failures for you”

Key Insight

Debt management must be continuous

8. Software Maintenance (Lifecycle Thinking)

From page 14 :

Types of maintenance:

Preventive → avoid future issues
Corrective → fix bugs
Adaptive → respond to changes
Perfective → improve performance
Applied Explanation

Example:

Preventive → add monitoring
Corrective → fix pipeline bug
Adaptive → handle new data format
Perfective → optimise performance
Key Insight

Maintenance is not reactive — it is strategic

9. Tools & Best Practices

From page 15 :

Version control (Git)
Monitoring (Grafana, Prometheus)
Testing (pytest)
Automation (CI/CD)
Applied Understanding

These tools support:

Early issue detection
Continuous improvement
Reliable deployments
10. Lab Integration (VERY IMPORTANT)

From the lab :

You are required to:

Build pipeline
Develop test decks
Document fully
Validate on real dataset
What this REALLY tests
Your ability to prevent technical debt
Your ability to test and validate systems
Your ability to document for maintainability
Key Insight

Poor documentation = technical debt

11. What This Topic Is REALLY Testing

You are being assessed on whether you can:

Recognise and manage system complexity
Prevent long-term failures
Maintain pipelines and systems
Balance delivery speed with quality
12. KSB Coverage Check (Explicit)
Knowledge (K)
K6 (System performance & reliability)
Understanding how debt impacts system stability
K7 (System design)
Understanding long-term system evolution
Skills (S)
S5 (Design & implementation)
Designing maintainable systems
S4 (Monitoring & evaluation)
Measuring and tracking technical debt
S2 (Data processing)
Maintaining reliable pipelines
Behaviours (B)
B1 (Responsibility)
Ownership of system quality
B2 (Continuous improvement)
Refactoring and optimisation
B4 (Professionalism)
Structured maintenance and documentation
13. Distinction-Level EPA Answer (Model Response)
Question:

“How would you identify, prioritise, and manage technical debt in a data engineering system?”

Model Answer (Distinction Level)

To identify, prioritise, and manage technical debt in a data engineering system, I would take a structured and continuous approach that balances delivery speed with long-term system reliability.

Firstly, I would identify technical debt by analysing both quantitative and qualitative indicators. Quantitative metrics such as code complexity, test coverage, and system performance would highlight areas of risk, while qualitative feedback from developers would reveal issues such as onboarding difficulty or fragile components.

Once identified, I would prioritise technical debt using an impact versus effort framework. High-impact, low-effort issues would be addressed first to quickly reduce risk, while more complex issues would be planned as part of longer-term improvements. I would also consider business risk, such as compliance implications or potential system failures, when prioritising work.

To manage technical debt effectively, I would integrate remediation into regular development cycles rather than treating it as a separate activity. This would include refactoring code, improving documentation, and implementing quality gates such as automated testing and CI/CD pipelines to prevent further debt accumulation.

In addition, I would apply software maintenance principles by categorising work into preventive, corrective, adaptive, and perfective maintenance. This ensures that the system remains stable, adaptable to change, and aligned with business needs over time.

Finally, I would track technical debt using a debt register and continuously reassess priorities as the system evolves. This ensures that technical debt is actively managed and does not accumulate to the point where it impacts system reliability or business operations.

This approach ensures that technical debt is not only identified and reduced, but also controlled over time, enabling the system to remain scalable, maintainable, and resilient.

Why This Hits Distinction
Covers identify → prioritise → manage → monitor
Links technical + business + risk
Shows continuous improvement mindset
Integrates tools, frameworks, and lifecycle thinking

14. Final Instructor Insight

At distinction level:

Technical debt is not a coding problem — it is a system design and decision-making problem over time

15. BIG Picture (Modules 8–10 Complete)

You can now explain:

Build pipelines (Module 8)
Govern and secure them (Module 9)
Deploy and monitor them (MLOps)
Maintain and improve them (Technical Debt)
Final Understanding

A complete data engineer builds systems that work today and are still reliable, maintainable, and scalable in the future
